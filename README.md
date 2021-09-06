# atelierpaper

Full stack <a href="https://atelierpaper.com">website</a> for an architecture firm in South Korea where:
1) architects can log in to submit their projects.
2) potential clients can explore and contact the architects they want to hire.

### Frontend
Coded using React, Bootstap, and DOMPurify (uber-tolerant XSS sanitizer) to prevent XSS attacks.
Used a responsive web design so the website will render beautifully on any devices.
Deployed it on AWS S3. The firm is based in Seoul, but has clients from all around the world. 
I used AWS CloudFront to optimize delivery speed by pushing the content to edge locations all around the globe.

### Backend
Coded using Node.js and PostgreSQL. Used cookie and session based authentification and authorization.
Deployed it on AWS EC2. Since the website have many users, I created multiple EC2 instances with a load balancer to optimize speed.
I used AWS CloudFront to push /api/* requests to the load balancer.
