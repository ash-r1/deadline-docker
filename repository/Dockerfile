FROM ubuntu:focal

ENV TZ=Asia/Tokyo
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

RUN apt-get update -y && apt-get install libssl-dev -y
COPY DeadlineRepository-*-linux-x64-installer.run .
COPY run.sh .

CMD ./run.sh
