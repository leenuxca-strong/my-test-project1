# NGINX Test Project
A lightweight sandbox for testing NGINX configurations and custom build modules.

## 🚀 Getting Started
Prerequisites: [Docker] (https://www.docker.com) or NGINX installed locally.

1. Clone the repo:

   git clone https://github.com

   cd nginx-test-app

2. Verify Configuration:

   Test your nginx.conf for syntax errors:

   nginx -t -c $(pwd)/nginx.conf

# If using Docker 

3. Run the app

   docker build -t nginx-test-app .

   docker run -p 8080:80 nginx-test-app5

5. Configuration Details

Port: Listens on port 8080.

Features: Static file serving, reverse proxy test, and custom 404 pages.

https://github.com/lebinh/nginx-conf/blob/master/README.md#:~:text=Links-,The%20Nginx%20Command,Force%20Trailing%20Slash

6. Verification

Run the following command to test the response:

curl -i localhost:8080

