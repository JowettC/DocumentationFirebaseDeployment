# DocumentationFirebaseDeployment
How to Deploy VueJS using Firebase
1. Create a project in firebase Console

![image](https://user-images.githubusercontent.com/57623021/130702745-68489be7-07f1-457d-89d9-247c31860051.png)

2. Install firebase tools through terminal (make sure NodeJS is installed)

```npm install -g firebase-tools```

3. Go to your project directory and create a production build of your web app

``` npm run build```

(This will create a dist folder)

4. Log into firebase in your console 

```firebase login```

This will prompt you to login via browser.

5. Set up configurations

``` firebase init```

Firebase offer a few services, we'll only be using hosting.
a. Pick a firebase project (will prompt you only on the first time)

b. Select hosting

![image](https://user-images.githubusercontent.com/57623021/130703602-aedc996d-158a-4ace-8969-db0b14f1278a.png)

c. set public directory to build folder (dist)

![image](https://user-images.githubusercontent.com/57623021/130703619-e8173e60-ebd9-40c3-833a-7f3058bf37ed.png)

d. Set the app as a single-page app? - OPTIONAL

![image](https://user-images.githubusercontent.com/57623021/130703713-528a94ab-63fa-414b-9de8-85eff984a8a3.png)

e. Automatic builds and deploy with GitHub set to no (this is new, optional for you to use in the future)

![image](https://user-images.githubusercontent.com/57623021/130703729-d798e91b-17ec-4549-b366-d809c191ed9d.png)

f. Do not overwrite existing index.html!
![image](https://user-images.githubusercontent.com/57623021/130703765-76d1a31c-3b45-4b30-ac00-725bc8e6542d.png)
Even if you do, you can just run ```npm run build``` again 


