FROM ubuntu:22.04 

WORKDIR  /yt.dlp

RUN apt update && apt install curl -y

COPY ./script.sh .

ENTRYPOINT ["./script.sh"]