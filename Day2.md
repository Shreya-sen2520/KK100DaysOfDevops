D2 === Temporary user setup with expiry

login to app server 1

ssh tony@stapp01

yes

password

-- verify james user exist or not

cat /etc/passwd | grep james

-- create user with expiry date

sudo useradd -e date mentioned james  or sudo chage -E date mentioned james

password

-- check expiry date of a user

sudo chage -l james