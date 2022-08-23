# amazon certificate manager (ACM)

- lets you provision, manage, and deploy public and private SSL/TLS certificates for use with AWS services
- ACM handles two kinds of certificates
  - **public** certificates provided by ACM -- **free**
  - **private** certificates you import ($400 / month)
- can be attached to API gateway, cloudfront, EB or ELB
- is not end-to-end-in-transit encryption since it terminates before reaching the instance
