# 1. node 설치
#FROM ubuntu:20.04
#RUN apt-get update
#RUN DEBIAN_FRONTEND=noninteractive apt-get install -y nodejs npm

#이미 Node 설치된 이미지 사용.
#FROM node:12

#최소한의 파일만 가진 버전(alpine)의 이미지 사용
FROM node:12-alpine

# 2. Nodejs 패키지 설치
WORKDIR /usr/src/app
RUN npm install

# 3. 소스 복사
COPY . /usr/src/app

# 4. WEB 서버 실행 (Listen 포트 정의)
EXPOSE 3000
CMD node app.js