# nodejs-server
Instructions to create NodeJS in AWS EC2 using nginx + Postgres

## Setting up a Node.js app on a Linux AMI on an AWS EC2 instance with Nginx
https://medium.com/@nishankjaintdk/setting-up-a-node-js-app-on-a-linux-ami-on-an-aws-ec2-instance-with-nginx-59cbc1bcc68c

## Enable HTTPS on AWS EC2 instance with Node.js and Nginx on Ubuntu server
https://medium.com/@victorleungtw/enable-https-on-aws-ec2-instance-with-node-js-and-nginx-on-ubuntu-server-15dad4864e11

## Setting up PostgreSQL
https://github.com/snowplow/snowplow/wiki/Setting-up-PostgreSQL

## Connecting to PostgreSQL
https://node-postgres.com/features/connecting

## Handle index.js changes

pm2 stop index.js
pm2 start index.js
pm2 startup
sudo env PATH=$PATH:/usr/bin /usr/lib/node_modules/pm2/bin/pm2 startup systemv -u ec2-user --hp /home/ec2-user
pm2 save
sudo service nginx restart
