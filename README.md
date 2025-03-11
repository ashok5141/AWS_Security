# AWS-Security-Specialty
- Course Material [Link](https://acloudguru-content-attachment-production.s3-accelerate.amazonaws.com/1681319452000-AWS_SECURITY_SPECIALTY_EXAM_STUDY_GUIDE.pdf)
- Notes for Security certification and understanding Document attacked in the Docs section [Online](https://d1.awsstatic.com/training-and-certification/docs-security-spec/AWS-Certified-Security-Specialty_Exam-Guide.pdf)

![AWS Security](https://raw.githubusercontent.com/ashok5141/AWS_Security/refs/heads/main/Docs/AWS%20Service.png)

| Domain | Topics | Weightings |
| :- | :- | :- |
| 1 | Threat Detection and Incident Response | 14 |
| 2 | Security Logging and Monitoring | 18 |
| 3 | Infrastructure Security | 20 |
| 4 |  Identity and Access Management | 16 |
| 5 | Data Protection | 18 |
| 6 | Management and Security Governance | 14 |

- **Thread Detection and Incident Response 14**
    - Design and Implement an incident response plan.
    - Detect secuirty threats and anomalies by using AWS services.
    - Respond to compromised resources and workloads.
- **Security Logging and Monitoring 18**
    - Design and implement monitoring and alerting to address security events.
    - Troubleshoot security monitoring and alerting.
    - Design and implement a logging solution.
    - Troubleshoot logging solution.
    - Design a log analysis solution.
- **Infrastructure Security 20**
    - Design and implement security controls for edge services.
    - Design and implement network security controls.
    - Design and implement security controls for compute workloads
    - Troubleshoot network security.
- **Identity and Access Management 16**
    - Design, implement, and troubleshoot authentication for AWS resources.
    - Design, implement, and troubleshoot authorization for AWS resources.
- **Data Protection 18**
    - Design and implement controls that provide confidentiality and integrity for data in transit.
    - Design and implement controls that provide confidentiality and integrity for data in rest.
    - Design and implement controls to manage the lifecycle of data at rest.
    - Design and implement controls to protect credentials, secrets, and cryptographic key materials.
- **Management and Security Governance 14**
    - Develop a strategy to centrally deploy and manage AWS accounts.
    - Implement a secure and consistent deployment strategy for cloud resources.
    - Evaluate the compliance of AWS resources.
    - Identity security gaps through architectural reviews and cost.
    

## Thread Detection and Incident Response

#### AWS Config
- AWS Config provides a detailed view of the configuration of AWS resources in your AWS account. This includes how the resources are related to one another and how they were configured in the past so that you can see how the configurations and relationships change over time.
- An AWS resource is an entity you can work with in AWS, such as an Amazon Elastic Compute Cloud (EC2) instance, an Amazon Elastic Block Store (EBS) volume, a security group, or an Amazon Virtual Private Cloud (VPC). For a complete list of AWS resources supported by AWS Config, see Supported Resource Types for AWS Config.

- Detailed Views
    - Detailed views of the configuration of your **AWS resources within AWS accounts**. Normalized data is delivered to S3 buckets.
- Historical Tracking
    - This including relation of resources as well as the configuration history from past periods of time. Essentially, it's a **Configuration recording timeline**.
- Not Prevention
    - The service is **not** meant to provide prevention of changes to resources, It's only for notifications of recorded changes.

> Ways to use AWS Config
- Resource Administration:- better governance of your AWS resources. Easily detect and notify of misconfigurations via fine-graned visibility into resources.
- Audit and Compliance:- Allows you to gain relevent audit data via the recorded historical configurations for all selected resources.
- Troubleshooting:- Cross-dependencies of AWS resources can be troublesome. Using Config allow us to view dependent resources affected by other potential resource changes.
- Security Analysis:- Better view into potential security weaknesses. View low-level changes to resources like AWS EC2 security groups(open ports) and IAM roles(Over-provisioned permissions)
