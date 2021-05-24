# Deploy to Heroku | English Guidline
Guidline Languages : Enligsh and Persian | English Language

## Very Simple Steps
1. Download Telegram from [here](https://telegram.org) , Then Install it .
2. Create your Telegram bot by [BotFather](https://t.me/BotFather)
3. if you don't installed Python on your System , Install Python from [here](https://www.python.org/downloads/windows/)
4. Install git from this [link](https://git-scm.com/download/win)
5. Register to Heroku from [here](https://signup.heroku.com/login)
6. Install Heroku CLI from [here](https://devcenter.heroku.com/articles/heroku-cli)

### [0] Step  [Optional]:

- For first , Git clone this repository and editing the files by below steps .

   ```shell
   git clone https://github.com/RexxarCompany/DeployToHeroku.git
   cd DeployToHeroku 
   
### [1] Step :

- Right click on boy.py and replace your source , then Save&Close boy.py .

### [2] Step :

- If you want rename bot.py , you should replace your custom name by editing *Procfile* file
 
   ```shell
   worker: python YourCustemName.py

### [3] Step :

- Add any moudels which you have included in your project to *requirements.txt*
  - Mine looks like this:

   ```shell
  future>=0.16.0
  certifi
  tornado>=5.1
  cryptography
  python-telegram-bot

### [4] Step :
- Change directory to where you have made these files
- now in git bash CLI, intialize a git

  ```shell
  git init
  
### [5] Step ::
- Install heroku CLI
- Next 

   ```shell
     heroku login
     heroku create app_name

- If you have already created app then select it:

   ```shell
     heroku git:remote -a app_name

 - Or else continue:
     ```shell
     git add -f bot.py Procfile requirements.txt __init__.py
 -  ```shell
     git commit -m "Added Files"

- If you want add anyfiles like "bot.jpg" to your project on heroku , Just add the name of that file at the end of the blow line

   ```shell
     git add -f bot.py Procfile requirements.txt __init__.py bot.jpg
 -  ```shell
     git commit -m "Added Files"
  
- Push files to heroku:

    ```shell
     git push heroku master
- If it is not working then try this one:

     ```shell
      git push heroku master --force
### At this point your bot should be running, you can check by
 
 -  ```shell
      heroku ps

- If it is not running then we have to reset dynos:
    ```shell
       heroku ps:scale worker=0
 -  ```shell
       heroku ps:scale worker=1
- Now it should be running fine! Enjoy :)  


### Do you need a Video Tutorial?
- Check Rexxar Youtube in [Here!](https://www.youtube.com/channel/UCJJfE0UeVfAVYsy90M7cdgQ)

Contact us : 

	Website : rexxar.ir
	Telegram : rexxar_ir
	Instagram : rexxar.ir

<div dir="rtl">
   
   # راه اندازی ربات تلگرام در وبسایت Heroku   |  زبان راهنما : فارسی
   زبان های راهنما : انگلیسی ، فارسی
	

	
   ## مراحل خیلی ابتدایی
   1. برنامه تلگرام را از [اینجا](https://telegram.org) دانلود کنید و سپس آن را نصب کنید.
   2. ربات تلگرام خود را توسط [BotFather](https://t.me/BotFather) بسازید.
   3. اگر پایتون در سیستم شما نصب نیست ، پایتون را از [اینجا](https://www.python.org/downloads/windows/) دانلود کنید و سپس نصب کنید.
   4. برنامه git را از طریق این [لینک](https://git-scm.com/download/win) دانلود و سپس نصب کنید.
   5. از طریق این [لینک](https://signup.heroku.com/login) در وبسایت Heroku ثبت نام کنید.
   6. برنامه Heroku CLI را از طریق این [لینک](https://devcenter.heroku.com/articles/heroku-cli) دانلود و نصب کنید.
   
   
   
   
   
   
   
   
   
   
   
   
   
   
   
   
   
   
   
   
   
   
   
   
   
   
   
   
   
   
   
   </div>
