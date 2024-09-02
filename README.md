# Portfolio Website Template with AWS Hosting 🎨

## 📚 Table of Contents
- [Overview](https://github.com/Sibi-Git/AWS-Portfolio-Builder/tree/main?tab=readme-ov-file#overview-)
- [Features](https://github.com/Sibi-Git/AWS-Portfolio-Builder/blob/main/README.md#features)
- [Installation](https://github.com/Sibi-Git/AWS-Portfolio-Builder/blob/main/README.md#installation)
- [Usage](https://github.com/Sibi-Git/AWS-Portfolio-Builder/blob/main/README.md#usage)
- [Architecture](https://github.com/Sibi-Git/AWS-Portfolio-Builder/blob/main/README.md#architecture)
- [Security](https://github.com/Sibi-Git/AWS-Portfolio-Builder/blob/main/README.md#security)
- [Monitoring and Logging](https://github.com/Sibi-Git/AWS-Portfolio-Builder/blob/main/README.md#monitoring-and-logging)
- [Customization](https://github.com/Sibi-Git/AWS-Portfolio-Builder/blob/main/README.md#customization)
- [Contributing](https://github.com/Sibi-Git/AWS-Portfolio-Builder/blob/main/README.md#contributing)
- [License](https://github.com/Sibi-Git/AWS-Portfolio-Builder/blob/main/README.md#license)
- [Contact](https://github.com/Sibi-Git/AWS-Portfolio-Builder/blob/main/README.md#contact)


## Overview 🌐
This project showcases a customizable portfolio website template hosted on AWS. The template is designed to be flexible and adaptable for various professional profiles, with a focus on a freelance photographer's portfolio. It leverages AWS services like EC2, Elastic Load Balancing (ELB), and Auto Scaling to ensure high availability and scalability.

## Features ✨
- **Responsive Design:** The template is fully responsive and works seamlessly across devices of all sizes.
- **AWS Hosting:** The website is hosted on AWS using EC2 instances, with Elastic Load Balancing and Auto Scaling to manage traffic and ensure uptime.
- **Customizable Sections:** Easily update content across multiple sections, including Home, About, Services, Portfolio, Testimonials, and Contact.
- **Interactive Elements:** Features interactive elements like image galleries, testimonial carousels, and a contact form.
- **SEO Optimized:** The template is optimized for search engines with clean, well-structured code.

## Installation 🛠️
### Deployment Steps
1. **Launch an EC2 Instance:**
   - Sign in to the AWS Management Console.
   - Launch a new EC2 instance using the Amazon Linux 2 AMI.
   - Configure the instance security group to allow HTTP and SSH access.
   - Deploy the website files to the EC2 instance.

2. **Set Up Elastic Load Balancing:**
   - Create an Application Load Balancer in the AWS Management Console.
   - Add your EC2 instances to the Load Balancer’s target group.

3. **Configure Auto Scaling:**
   - Create an Auto Scaling group in AWS.
   - Attach your Load Balancer to the Auto Scaling group.
   - Set scaling policies to manage the number of running instances based on traffic.

4. **Set Up DNS with Route 53 (Optional):**
   - Configure a domain name using AWS Route 53 for easy access to your portfolio website.

5. **Monitor and Optimize:**
   - Use CloudWatch to monitor the performance and health of your instances.
   - Adjust Auto Scaling and Load Balancing settings as needed.

## Usage 💻
### Customize Content:
- Update the HTML, CSS, and JS files in the `index.html`, `style.css`, and `custom.js` files to personalize the template.
- Replace placeholder images and text with your own content.

### Deploy to AWS:
- Follow the deployment steps outlined above to host your customized portfolio on AWS.

## Architecture 🏗️
- **Multi-AZ Deployment:** The EC2 instances are deployed across multiple Availability Zones (AZs) for high availability.
- **Load Balancing:** The ELB automatically distributes incoming traffic across multiple EC2 instances, ensuring no single instance is overwhelmed.
- **Auto Scaling:** Automatically scales the number of EC2 instances based on the current traffic load, providing both cost efficiency and reliability.
- **DNS Management:** Optionally use Route 53 for domain name management, making it easier to access your portfolio with a custom domain.

## Security 🔒
- **IAM Roles:** Secure the AWS environment by assigning the least-privilege IAM roles to EC2 instances.
- **Security Groups:** Control inbound and outbound traffic to your instances using security groups, only allowing necessary traffic (e.g., HTTP, HTTPS, SSH).
- **SSL/TLS:** Implement SSL/TLS certificates to encrypt traffic between the client and server, ensuring secure communication.

## Monitoring and Logging 📊
- **CloudWatch:** Set up CloudWatch to monitor CPU usage, memory, disk I/O, and network traffic.
- **AWS CloudTrail:** Use CloudTrail to log all API requests and account activity, providing an audit trail for security analysis and troubleshooting.
- **Logs:** Store application and server logs in CloudWatch Logs or an S3 bucket for long-term storage and analysis.

## Customization 🎨
Users can customize various parts of the code:
- **`index.html`:** Modify the content and structure of the website. Customize sections like Home, About, Services, Portfolio, Testimonials, and Contact.
- **`style.css`:** Adjust the styling, including colors, fonts, and layouts, to match your branding.
- **`custom.js`:** Add interactivity, handle animations, and manage client-side logic.

For example, you can change the title of the website in `index.html`:

```html
<title>Sibi Marappan - Portfolio</title>
```

And modify the main heading:

```html
<h1>Hello, I'm Sibi Marappan</h1>
```

## Contributing 🤝
Contributions are welcome! Feel free to submit issues or pull requests to improve the template.

## License 📄
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact 📧
For any questions or support, please reach out to:
- **Name:** Sibi Marappan
- **Email:** msibi.mail@gmail.com
- **LinkedIn:** [Sibi Marappan](https://www.linkedin.com/in/sibi-marappan/)
