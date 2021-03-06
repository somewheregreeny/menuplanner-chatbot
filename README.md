# ๐ menuplanner-chatbot
<p>
  <img src="https://img.shields.io/badge/Amazon AWS-232F3E?style=flat&logo=Amazon AWS&logoColor=white">
  <img src="https://img.shields.io/badge/Spring Boot-6DB33F?style=flat&logo=Spring Boot&logoColor=white">
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=Python&logoColor=white">
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat&logo=MySQL&logoColor=white">
  <img src="https://img.shields.io/badge/KaKaoTalk-FFCD00?style=flat&logo=KaKaoTalk&logoColor=white">
</p>

ํ๊ตญ๊ณตํ๋ํ๊ต TIP ์งํ ์๋น๊ณผ E๋ ์๋น์ ๋ฉ๋ด๋ฅผ ์๋ ค์ฃผ๋ ์ฑ๋ด ํ๋ก์ ํธ

## Description
- ์๋น๋ฉ๋ด๋ฅผ ๋ณด๊ธฐ ์ํด ํ๊ตญ๊ณตํ๋ ์ฑ์ผ๋ก ๋ค์ด๊ฐ์ ์ฌ์ง์ผ๋ก ๋ด์ผํ๋ ๋ถํธํจ์ ํด๊ฒฐํ๊ธฐ ์ํด์ ์ ์ํ์ต๋๋ค.
- ์นด์นด์ค ์ฑ๋ด์ ์ด์ฉํด ๋ฉ์์ง๋ก ์ค๋์ E๋ ์๋น๊ณผ TIP ์งํ ์๋น์ ๋ฉ๋ด๋ฅผ ์ ๊ณตํฉ๋๋ค.

- [์ฑ๋ด ๋ฐ๋ก ๊ฐ๊ธฐ](https://pf.kakao.com/_hwWLb)

## Architecture

<img src="./images/architecture.png">
<img src="./images/database_architecture.png">

## Screenshot
<div>
  <img height=875 src="./images/tip.png">
  <img height=875 src="./images/eblock.png">
</div>

## How it works?

1. spring ์๋ฒ๋ฅผ ์คํํ๋ฉด API๋ฅผ ์ด์ฉํด aws lambda์ ์ฌ๋ ค ๋์ ํ์ด์ฌ ํจ์์๊ฒ ํ์ผ ์ด๋ฆ์ ํ์ฑํ๋ผ๊ณ  ์์ฒญํฉ๋๋ค.
2. ์๋ฒ๋ ํ์ผ ์ด๋ฆ, bookCode๋ฅผ ๋ฐ์์ ๋ค์ E๋, TIP ์๋น์ ๋ฉ๋ด๋ค์ ํ์ฑํ๋ผ๊ณ  ์์ฒญํฉ๋๋ค.
3. ์๋ฒ๋ ๋ฉ๋ด๋ค์ ๋ฐ์์ ์ ๋ถ RDS๋ฅผ ์ด์ฉํ DB(mysql)์ ์ ์ฅํฉ๋๋ค.
4. ์นด์นด์ค ์ฑ๋ด์ผ๋ก๋ถํฐ ์์ฒญ์ด ์ค๋ฉด, ๊ทธ์ ๋ง๋ ๋ฉ์์ง ํ์์ json ํํ๋ก ๋ฐํํฉ๋๋ค.
5. ์์์ผ 7์ 0๋ถ์ด ๋๋ฉด ์๋จ ์๋ฐ์ดํธ๋ฅผ ์ํด 10๋ถ๋ง๋ค DB์ ์ ์ฅ๋์ด ์๋ ํ์ผ ์ด๋ฆ๊ณผ ํ์ฑํ ํ์ผ ์ด๋ฆ์ ๋น๊ตํฉ๋๋ค.
6. ๋ฌ๋ผ์ก๋ค๋ฉด, ๋ฉ๋ด๊ฐ ์๋ก๋ ๋ ๊ฒ์ผ๋ก 1๋ฒ๋ถํฐ ๋ค์ ์ํํฉ๋๋ค.

## Run server

- ์์ธํ ์ค๋ช์ ๋๋ ํ ๋ฆฌ์ README๋ฅผ ์ฐธ์กฐํด์ฃผ์ธ์.

- [spring ์๋ฒ](https://github.com/somewheregreeny/menuplanner-chatbot/tree/main/menuplanner-chatbot-api)
- [aws lambda python](https://github.com/somewheregreeny/menuplanner-chatbot/tree/main/aws-rambda-python)
