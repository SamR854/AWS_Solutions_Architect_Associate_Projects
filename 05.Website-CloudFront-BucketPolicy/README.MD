# AWS Website Hosting with CloudFront and S3 Bucket Policy

## Project Overview

This project demonstrates how to securely host a static website using Amazon S3 and Amazon CloudFront.

The solution uses CloudFront as a Content Delivery Network (CDN) to improve website performance, reduce latency, and provide secure access to content stored in an Amazon S3 bucket.

## Business Requirement

A company requires a website hosting solution that:

- Delivers content globally with low latency
- Improves website performance
- Enhances security
- Restricts direct access to the S3 bucket
- Scales automatically with demand

## AWS Services Used

- Amazon S3
- Amazon CloudFront
- AWS IAM
- S3 Bucket Policies

## Solution Architecture

User → CloudFront Distribution → Amazon S3 Bucket

CloudFront caches content at edge locations and retrieves files securely from Amazon S3.

## Components

### Amazon S3

Hosts the website files, including:

- HTML
- CSS
- JavaScript
- Images

### Amazon CloudFront

Provides:

- Global content delivery
- Edge caching
- Reduced latency
- Improved performance
- Enhanced security

### S3 Bucket Policy

Controls access to website content and restricts direct access to the S3 bucket.

### IAM

Provides secure administration and access management.

## Implementation Steps

1. Create an Amazon S3 bucket.
2. Upload website content.
3. Configure bucket permissions.
4. Create a CloudFront distribution.
5. Set the S3 bucket as the origin.
6. Configure caching behavior.
7. Apply an S3 bucket policy.
8. Test content delivery through CloudFront.
9. Verify security settings.
10. Validate website accessibility.

## Security Design

A key objective of this project was preventing unrestricted public access to content.

Security controls included:

- Controlled bucket permissions
- Bucket policy configuration
- Access through CloudFront
- Principle of least privilege using IAM

## Benefits of CloudFront

- Faster content delivery
- Reduced latency
- Improved user experience
- Global availability
- Scalable architecture
- Increased security

## Skills Demonstrated

- Amazon S3 Administration
- CloudFront Configuration
- Content Delivery Networks (CDN)
- Bucket Policy Management
- IAM Permissions
- Website Hosting
- Security Best Practices
- Performance Optimization

## Challenges and Lessons Learned

### Challenge

Configuring bucket permissions while maintaining secure access to website content.

### Solution

Implemented bucket policies that allowed CloudFront access while maintaining appropriate security controls.

### Key Learning

CloudFront improves both performance and security when combined with Amazon S3 static website hosting.

## Future Improvements

- Configure HTTPS using AWS Certificate Manager
- Add a custom domain using Route 53
- Enable CloudFront logging
- Implement Web Application Firewall (AWS WAF)
- Configure monitoring using CloudWatch

## Project Outcome

Successfully deployed a static website using Amazon S3 and Amazon CloudFront while implementing bucket policies to control access. The solution demonstrated how AWS services can be combined to create a secure, scalable, and high-performance website hosting architecture.

## Key AWS Concepts Demonstrated

- Content Delivery Networks (CDN)
- Edge Locations
- S3 Static Website Hosting
- Cloud Security
- IAM Permissions
- Bucket Policies
- Scalability
- Performance Optimization
