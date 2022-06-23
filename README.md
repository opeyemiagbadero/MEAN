## MEAN STACK DEPLOYMENT TO UBUNTU IN AWS ##

I spun up an EC2 on my AWS account for project 4, used the  chmod 400 opeyemi.pem and sshed into my server.

![Screenshot 2022-06-23 at 21 26 42](https://user-images.githubusercontent.com/79456052/175393407-445418d9-eb62-496c-891b-104e846f2c10.png)


Step 1: Install NodeJs

I updated and upgraded ubuntu usung the sudo apt update and sudo apt upgrade commands

![1  sudo apt update and sudo apt upgrade](https://user-images.githubusercontent.com/79456052/175394671-eb6c4ae7-d086-42fe-96b3-f425c79981e5.png)

![2  sudo apt upgrade](https://user-images.githubusercontent.com/79456052/175394687-3c94565b-4d0f-48bb-a4df-6e3e595246d3.png)

I added the certificates and installed NodeJS on the server using the  sudo apt install -y nodejs
![3  Add certificates](https://user-images.githubusercontent.com/79456052/175394817-922f767d-e9f8-49a6-8634-e91212dd6633.png)

![4  Install NodeJS](https://user-images.githubusercontent.com/79456052/175395849-3394dfec-3577-44b7-975a-4ec4b47be21e.png)
 
 Step 2: I installed MongoDB, started the server and verified that the server was up and running

![5  Install MongoDB](https://user-images.githubusercontent.com/79456052/175396509-1022a79d-0890-41e2-8272-3ec63200c727.png)

followed by installing Npm-Node package manager

![6  Install npm - Node package manager](https://user-images.githubusercontent.com/79456052/175396919-a98a1443-0ba4-40fe-807d-a1018a8585f6.png)

I  installed the body-parser, created a Book directory and initiated npm in the book directory.A file named server .js was opened in the book directory  and the configuration as given in the documentation was copied and pasted into the server.js file.

![7  Install body-parser and init npm in the Books dir](https://user-images.githubusercontent.com/79456052/175397129-22aebd11-2293-4e17-bcaa-ca77116a8e16.png)

Step 3: Install Express and set up routes to the server by installing mongoose, using the *sudo npm install express mongoose*  command followed by creating a folder called apps in the books command and creating a file called routes.js in the apps directory. The routes.js file was opened and a set configuration as given in the PBL4 documentation was copied and pasted into the route.js file.

In the ‘apps’ folder, I created a folder named models, followed by creating  a file named book.js. I copied and pasted the code given in the PBL4 documentation into the ‘book.js’ file and saved it.


![8 INSTALL EXPRESS AND SET UP ROUTES TO THE SERVER](https://user-images.githubusercontent.com/79456052/175396968-d9e4632d-cd19-41c9-89d6-34619333b436.png)


![8](https://user-images.githubusercontent.com/79456052/175396955-4f8e02cf-c474-4b3f-963e-5bbcbff0938a.png)

Step 4- Accessing the routes with Angular JS

I created a a folder name public in the books directory and added a file called script.js. A configuration as given in the PBL 4 documentation was copeid, pasted and saved in the file. In the public folder, I created a file named index.html, opened the file  and copied, pasted and saved a set of configuration as  given in the PBL4 documentation. 

I started the server bu running the *node server.js* command,  On the AWS console, I edited the inbound rules of the security group  on the server so that TCP port 3300 can be made  open for traffic

![10](https://user-images.githubusercontent.com/79456052/175396985-8f5456b7-717f-44da-b8e0-f5a0304dae28.png)

The last step was opening up the public ip address of the server using port 3300 i.e http://3.84.19.60:3300 on my chrome browser and inputting a set of data on the web book register application of the browser.


![11](https://user-images.githubusercontent.com/79456052/175406383-60e72bc4-78f4-42f0-9b15-ee762f237952.png)




