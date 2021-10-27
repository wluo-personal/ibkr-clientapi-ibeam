# ibkr-client
This project is to maintain docker containers to launch ibkr client

# build
sudo docker build -t ibkrtest .

# run
sudo docker run --env-file=/home/wei/.sec/ibkrsecrets_paper.list -p 5000:5000 --name ibtest ibkrtest

sudo docker run -d --env-file=/home/wei/.sec/ibkrsecrets_paper.list -p 5000:5000 --name ibtest ibkrtest > /home/wei/ibtest.log
