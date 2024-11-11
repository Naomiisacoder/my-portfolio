# personal-website
![GitHub repo size](https://img.shields.io/github/repo-size/codewithsadee/vcard-personal-portfolio)

## Documentation about this project. 

### Step 1: Setting Up Project Repository on GitHub
a. Created a New Repository on GitHub and named it personal-website <br>
b. Clone the repository to my local machine 
```bash
git clone https://github.com/your-username/portfolio-website.git
cd portfolio-website
```
<br>

### Step 2: How I built my Docker image <br>
a. I made use of NGINX for this Static website:
# nginx:alpine (a lightweight web server) to serve this static files.

### Dockerfile

```bash
# Use a lightweight web server to serve static files
FROM nginx:alpine
COPY . /usr/share/nginx/html
EXPOSE 80
```
#### NOTE: A Dockerfile is needed to package your application so it can run consistently anywhere.
<br>
b. Testing Locally: I built and ran the Docker image locally to make sure everything works before deploying following the steps below:

### Bash
```bash
docker build -t portfolio-site .
docker run -p 8080:80 portfolio-site  # For NGINX
docker run -p 8080:8080 portfolio-site  # For Flask
```




### Step 3: GitHub Pages


### Step 4: Challenges I encountered.



vCard is a fully responsive personal portfolio website, responsive for all devices, built using HTML, CSS, and JavaScript.

## Demo

![image](https://github.com/user-attachments/assets/9daefc8a-4d46-42c9-8c1e-acb039f26d23)

![image](https://github.com/user-attachments/assets/830183f9-8cf9-464c-bfa1-46291035aea7)


## Prerequisites

Before you begin, ensure you have met the following requirements:

* [Git](https://git-scm.com/downloads "Download Git") must be installed on your operating system.

## Installing vCard

To install **vCard**, follow these steps:

Linux and macOS:

```bash
sudo git clone https://github.com/codewithsadee/vcard-personal-portfolio.git
```

Windows:

```bash
git clone https://github.com/codewithsadee/vcard-personal-portfolio.git
```

## Contact

If you want to contact me you can reach me at [Twitter](https://www.x.com/MaryCybSec).

## License

This project is **free to use** and does not contains any license.

