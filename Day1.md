Day1  -- Linux user setup with Non-interactive shell

Create a user name john with Non-interactive shell on app server 1

-- login app server 1

ssh tony@stapp01

yes

password

-- root user 

sudo su - or sudo -i

password 

-- verify john user exist or not

cat /etc/passwd | grep john

-- create john user

sudo adduser john --shell /sbin/nologin

-- validate

cat /etc/passwd | grep john