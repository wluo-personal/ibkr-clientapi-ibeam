# ibkr-client
This project is to maintain docker containers to launch ibkr client

# build
sudo docker build -t toneymall/ibkrclient:v1.0.0 .

# run

sudo docker run -d --env-file=/home/wei/.sec/ibkrsecrets_paper.list -p 5000:5000 --name ibpaper toneymall/ibkrclient:v1.0.0

sudo docker run -d --env-file=/home/wei/.sec/ibkrsecrets_prod.list -p 5001:5000 --name ibprod toneymall/ibkrclient:v1.0.0