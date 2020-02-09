FROM debian:sid

RUN apt-get update -y

RUN apt-get install -y iperf procps

CMD ["iperf", "-s"]
