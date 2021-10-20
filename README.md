<h2>Java Based Micro Services ECommerce Application</h2> 
<h2>This application can be executed in following modes</h2> 
<ol>
  <li>Run the application without APM Agent attached to it</li>
  <li>Run the application with APM Agent using volume mount approach</li>
  <li>Run the application using embedded APM Agent</li>
</ol>
<h2>Pre-requisites</h2> 
<ul>
  <li>Make sure you have JAVA 8 or JRE 8 installed.</li>
  <li>Make sure you have maven installed.</li>
  <li>Make sure you have git installed.</li>
  <li>Make sure you have docker-compose installed.</li>
</ul>
<h2>Compile and Build Application</h2> 
<b><u>Step 1 :</u></b> To clone this application
<pre><code>git clone https://github.com/eginnovations/webstore-micro-services-app
</code></pre>
<b><u>Step 2 :</u></b> Navigate to application home directory 
<pre><code>cd webstore-micro-services-app
</code></pre>
<b><u>Step 3 :</u></b> To build the application 
<pre><code>mvn clean package
</code></pre>

<h2>Run the application without APM Agent </h2>

<b><u>Step 1 :</u></b> Navigate to application home directory (webstore-micro-services-app)

<b><u>Step 2 :</u></b> To build docker images and run all the application containers

<pre><code>docker-compose up -d --build
</code></pre>

<b><u>Step 3 :</u></b> To ensure all containers started and running <code>docker ps -a</code>

<b><u>Step 4 :</u></b> Open the browser and access the application using "http://DOCKER_HOST_IP:8070/webstore"

<h2>Run the application with APM Agent using volume mount (Only Linux)</h2>

<b><u>Step 1 :</u></b> Navigate to directory "webstore-micro-services-app/btm_volume_mount/"

<b><u>Step 2 :</u></b> To build docker images and run all the application containers

<pre><code>docker-compose up -d --build
</code></pre>

<b><u>Step 3 :</u></b> To ensure all containers started and running <code>docker ps -a</code>

<b><u>Step 4 :</u></b> Open the browser and access the application using "http://DOCKER_HOST_IP:8070/webstore"

<h2>Run the application using embedded APM Agent (APM Agent embedded inside container image)</h2>

<b><u>Step 1 :</u></b> Navigate to directory "webstore-micro-services-app/btm_embedded/"

<b><u>Step 2 :</u></b> To build docker images and run all the application containers

<pre><code>docker-compose up -d --build
</code></pre>

<b><u>Step 3 :</u></b> To ensure all containers started and running <code>docker ps -a</code>

<b><u>Step 4 :</u></b> Open the browser and access the application using "http://DOCKER_HOST_IP:8070/webstore"

<h2>To stop the application</h2>

<b><u>Step 1 :</u></b> Navigate to directory where the docker-compose.yml is present and run the below command.

<pre><code>docker-compose down
</code></pre>

<h2>THIS IS FOR THE PURPOSES OF TRAINING OR INTERNAL USE ONLY, DO NOT SHARE TO CUSTOMER/PROSPECT/OTHERS</h2> 

