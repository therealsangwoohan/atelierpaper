# atelierpaper

Full stack <a href="https://atelierpaper.com">website</a> for an architecture firm in South Korea.

### Frontend
Coded using React, Bootstap, and DOMPurify (uber-tolerant XSS sanitizer) to prevent XSS attacks.
Deployed it on AWS S3. The firm is based in Seoul, but has clients from all around the world. 
I used AWS CloudFront to optimize delivery speed by pushing the content to edge locations all around the globe.

### Backend
Coded using Node.js and PostgreSQL.
Deployed it on AWS EC2. Since the website have many users, I created multiple EC2 instances with a load balancer to optimize speed.
I used AWS CloudFront to push /api/* requests to the load balancer.
