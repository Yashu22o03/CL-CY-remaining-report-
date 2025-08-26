## Task 10 :  Create an application on EC2 instance

**Amazon EC2** is a cloud service that lets you **run virtual computers (called instances)** in the cloud. You can use EC2 to run websites, applications, databases, or anything you'd normally run on a computer — but without owning any hardware.

### Key Concepts :
1. **Instance :** An **Instance** is a virtual server. It runs an operating system like Linux or Windows and can host anything - websites, apps, APIs, databases, etc. 
2. **AMI (Amazon Machine Image) :** An **AMI** is a pre-configured template used to launch an EC2 instance. It includes the operating system and software you want on the instance. 
3. **Security Group :** A **security group** acts like a firewall for your instance. It controls what traffic is allowed in and out. 
4. **Elastic IP :** An **Elastic IP** is a static IP address you can assign to your EC2 instance. It's useful if your app or website needs a consistent IP address for users or DNS.

 I launched an EC2 instance on AWS using an Ubuntu image and configured it to host a simple Flask web application. I installed Python and Flask inside a virtual environment to avoid conflicts with the system-managed environment. 
 
 
 The Flask app was designed to return a basic "Hello from EC2!" message, and I ensured it was accessible over the internet by adjusting the instance’s security group to allow inbound traffic on port 5000. The app was successfully tested via the instance’s public IP. This exercise demonstrated key skills in setting up cloud infrastructure, configuring a virtual environment, and deploying a basic web service on AWS EC2.


Below is the screenshot of the instance I created :
[![Screenshot-2025-06-01-232507.png](https://i.postimg.cc/dtCP88R2/Screenshot-2025-06-01-232507.png)](https://postimg.cc/rKqPTRPs)
Below is the command line of Ubuntu that I set up using Git Bash :
[![Screenshot-2025-06-01-233327.png](https://i.postimg.cc/0N8TRFTn/Screenshot-2025-06-01-233327.png)](https://postimg.cc/VJVGXGL0)
Below is the output screen on a different tab :
[![Screenshot-2025-06-01-232903.png](https://i.postimg.cc/7Z1FRwWb/Screenshot-2025-06-01-232903.png)](https://postimg.cc/3kRf457H)
