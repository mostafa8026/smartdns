# SmartDNS
You can easily set your favorite dns by deploying this repository as a DNS server.

<h2>Step 1:</h2>
prepare a linux server (ubuntu/debian) with a PUBLIC IP address available on it.<br/>
Install docker on it, you can use the following link if you use ubuntu 20.04:<br/>
https://support.netfoundry.io/hc/en-us/articles/360057865692-Installing-Docker-and-docker-compose-for-Ubuntu-20-04

<h2>Step 2:</h2>
Clone this repo onto your server using this command (you have to install git first using "sudo apt install git"):<br/>
<code>$sudo git clone https://github.com/arezoomaleki/smartdns.git</code>

<h2>Step 3:</h2>
Finally you can provide your Server IP by simply copying the .env.sample.

<code>$ cd smartdns</code><br/>
<code>$ sudo cp .env.sample .env</code><br/>
<code># edit the IP field to your server IP</code><br/>
<code>$ docker compose up --build -d</code><br/>
<br/><br/>
<div style='color: red'>
  <b>P.S:</b><br/>
  <b>Everytime you add a domain into dnsmasq.conf and domains.txt you have to run the <code>docker compose up --build -d</code></b>
<div>
