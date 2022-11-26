# Yukki Multi Spam Bot 

<p align="center">
  <img src="https://telegra.ph/file/9daafeb39193a4a22ee5c.jpg">
</p>

## 🚀 Deploy on Heroku 
[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://dashboard.heroku.com/new?template=https%3A%2F%2Fgithub.com%2FYukkiBot%2FYukkiMultiSpamBot)

You can Use these [API ID and API HASH](https://t.me/OfficialYukki/135) while deploying

## String Session
No Requirement of API ID and API HASH

   - Generate on Repl [![Run on Repl.it](https://repl.it/badge/github/YukkiBot/YukkiSpamBot)](https://replit.com/@YukkiBot/YukkiSpamBot)
   - Termux : `sh -c "$(curl -fsSL https://da.gd/YukkiBot)"` (Use `python string_session.py` next time to generate another string.)
shikhar@MacBook~ $ git clone https://github.com/TeamYukki/YukkiChatBot

shikhar@MacBook~ $ cd YukkiChatBot

shikhar@MacBook~ $ pip3 install -r requirements.txt

shikhar@MacBook~ $ mv sample.env .env

## Support Group
   - Join [Yukki Support Group](https://t.me/officialyukki) for any assistance.
## Credits
   - Thanks to [Yukki Team](https://t.me/officialyukki).
   
   
   FROM debian:latest

RUN apt update && apt upgrade -y
RUN apt install git curl python3-pip -y
RUN pip3 install -U pip
RUN mkdir /app/
WORKDIR /app/
COPY . /app/
RUN pip3 install -U -r requirements.txt
CMD python3 Yukki.py
