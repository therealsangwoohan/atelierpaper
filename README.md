# atelierpaper

Full-Stack <a href="https://atelierpaper.com">website</a> for an architecture firm in South Korea where:
1) Architects can log in to submit their projects.
2) Potential clients can explore and contact the architects they want to hire.

### Frontend
It was coded using React and Bootstrap. I also used DOMPurify (uber-tolerant XSS sanitizer) to prevent XSS attacks. Used a responsive web design so the website would render beautifully on any device. It was deployed on AWS S3. The firm is based in Seoul but has many international clients. I used AWS CloudFront to optimize delivery speed by pushing the content to edge locations all around the globe.

### Backend
It was coded using Node.js and PostgreSQL. Used cookie and session-based authentification and authorization. It was deployed on AWS EC2. Since the website has many users, I created multiple EC2 instances with a load balancer to optimize speed. I used AWS CloudFront to push /api/* requests to the load balancer.
