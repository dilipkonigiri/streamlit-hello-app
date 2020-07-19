# Streamlit Web App
![Python 3.6](https://img.shields.io/badge/Python-3.6-brightgreen.svg) ![Streamlit](https://img.shields.io/badge/Streamlit-Library-orange.svg)<br>

## About Streamlit
• Streamlit’s open-source app framework is the easiest way for data scientists and machine learning engineers to create beautiful, performant apps in only a few hours!  All in pure Python. All for free.<br>

• If you want to view the deployed model, click on the following link:<br>
Deployed at: https://streamlit-hello-app-sk.herokuapp.com/ <br>



### Streamlit deployment steps

1. Create a repository on github and clone in your PC
2. Navigate to that folder in the terminal
3. Make a file named app.py
4. Make a file named Procfile and paste this

	web: sh setup.sh && streamlit run app.py

5. Make a file named requirements.txt
6. Make a file named setup.sh and paste this


mkdir -p ~/.streamlit/

echo "\
[server]\n\
headless = true\n\
port = $PORT\n\
enableCORS = false\n\
\n\
" > ~/.streamlit/config.toml


7. heroku login
   heroku create
   git add .
   git commit -m "Some message"
   git push heroku master
