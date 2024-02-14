### Create a simple script file , with some data present it and push it Jenkins connected to your GitHub repository. When a commit is made to your repo, automatically build must get triggered from Jenkins and the output must be shared to me via email."

I have used the same application file already available.
[ https://github.com/Surya-hu/mycicdpipeline]

Using Jenkins I have created new project called "mycicdpipeleine"
As shown below

![image](https://github.com/Surya-hu/jenkins_tasks/assets/119995742/d3b5be5b-cd0b-49ee-8a18-90c19a2c6ec2)

Using configure option selected `github project` and build trigger as `GitHub hook trigger for GITScm polling`

![image](https://github.com/Surya-hu/jenkins_tasks/assets/119995742/0c596e21-767c-4617-bfb4-e93b3c954ce7)

After that will need to goto github repo --> setting --> webhook and configure as below:

1. need to take the ip address of jenkins and add `/github-webhook/` at the end --> click `ok`
2. select format as JSON
3. then click `ok/create`

![image](https://github.com/Surya-hu/jenkins_tasks/assets/119995742/6c369a97-825d-4d78-80ef-4d61b6dc3033)

Before editing the code git repo:

![image](https://github.com/Surya-hu/jenkins_tasks/assets/119995742/c9237c07-ee5c-41a2-9274-5d51971c2897)

webpage:
![image](https://github.com/Surya-hu/jenkins_tasks/assets/119995742/51264d35-a839-4098-873e-49f47a08e671)

Jenkins page with the last commit number(#10):

![image](https://github.com/Surya-hu/jenkins_tasks/assets/119995742/aa9a18f2-6492-4f5a-85c2-f0a07a7ca6ff)

new commit pushing:

![image](https://github.com/Surya-hu/jenkins_tasks/assets/119995742/5799167a-0b55-4a92-8304-10b16c365d2c)

New build triggered automatically as shown below:

![image](https://github.com/Surya-hu/jenkins_tasks/assets/119995742/2bc2b89e-3078-4c6a-a2b3-2b832c774522)

![image](https://github.com/Surya-hu/jenkins_tasks/assets/119995742/e40b0399-a3f3-4f41-b372-b495173ab527)

Container is running:

![image](https://github.com/Surya-hu/jenkins_tasks/assets/119995742/cfd5a22b-3804-4b68-8235-91e7b8db2c7c)

webpage after commiting new chnages:

![image](https://github.com/Surya-hu/jenkins_tasks/assets/119995742/4b8f9b85-1b1d-4698-91e8-12085b11c779)

Email Config:

1. Downloaded `Email Extension Plugin` from manage jenkins --> plugin --> avialable pugins --> Search for Email Extension Plugin.

2. From manage jenkins --> system --> E-mail notification changed below settings:

![image](https://github.com/Surya-hu/jenkins_tasks/assets/119995742/7e8bdce3-eb9f-4cf8-a7eb-82d7b8730cf1)

![image](https://github.com/Surya-hu/jenkins_tasks/assets/119995742/05648fd2-b95d-4958-bec8-6103cbb3e1a9)

3. Then went and configured two-way authentication in my gmail account
4. Then edited Jenkins file with mail subject and to addresses.
5. Made a push frm git repo and found the email notification as shown below.

![image](https://github.com/Surya-hu/jenkins_tasks/assets/119995742/779355ca-f0f8-4681-9993-44f32da49439)




