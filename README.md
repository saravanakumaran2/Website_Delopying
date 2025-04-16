# Website Deploying 
  
This is one of my early DevOps practice projects where I learned how to **deploy a static website** from source code to a running web server.

---

## What I Did in This Project

- Wrote a small static website (HTML/CSS files)
- Organized the code inside this repo
- Set up a **web server** (probably Apache or Nginx)
- Used **SCP or SSH** to copy the site to the remote server
- Hosted the site and tested it in a browser

---

## The Goal

I wanted to learn **how a simple website gets deployed** from my machine or GitHub to a real server, where anyone can open it in a browser.

---

## What’s Inside the Repo

```bash
.
├── index.html       
├── styles.css         
├── images/            
└── README.md         
```

---

## Notes 

- Always make sure the destination path on the server is correct (like `/var/www/html`)
- Use `scp` like:
  ```bash
  scp -r * user@server_ip:/var/www/html
  ```
- Make sure the web server is started:
  ```bash
  sudo systemctl start apache2   # or nginx
  ```
- Use correct file permissions so the server can read the files

---


