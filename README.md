# qrcode-checks
scan qr code to fill out a web form that some action has been completed (such as a check of a building)


## requirements
> assumes debian 10

```
echo "deb http://http.us.debian.org/debian/ testing non-free contrib main" >> /etc/apt/sources.list
echo "deb http://repo.mongodb.org/apt/debian buster/mongodb-org/5.0 main" | tee /etc/apt/sources.list.d/mongodb-org-5.0.list
echo "alias python=python3" >> ~/.bashrc
source .bashrc

wget -qO - https://www.mongodb.org/static/pgp/server-5.0.asc | apt-key add -


apt update && apt dist-upgrade -y

apt install python3-pip mongodb-org nodejs npm -y
```

## npm
```
npm install axios bootstrap
npx create-react-app frontend
```

## run app

```
uvicorn main:app --host 0.0.0.0 --reload
npm start
```
