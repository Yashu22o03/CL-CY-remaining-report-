## Task 9 : AWS CloudFront - Serve content from multiple S3 buckets

**Amazon S3** is a cloud-based **object storage service**. That means it lets you **store and retrieve any amount of data** (like files, images, videos, documents) from anywhere on the web, at any time. Imagine it like an **online folder or drive**, but way more powerful and scalable.


### Key Concepts :
1. **Bucket :** A **bucket** is like a container or folder in S3 where you store your files. Every file you upload must go into a bucket. Each bucket has a unique name (across all AWS users), and you choose the AWS region where it's stored.
2. **Object :** An **object** is the actual file you store in a bucket. It could be anything - a document, image, video, or backup. Along with the file itself, each object also has metadata and a unique identifier called a "key".
3. **Key :** The key is the name used to identify an object within a bucket. It works like a file path. 
4. **Region :** When you create a bucket, you must choose a **region**. In my case, it was `ap-south-1` which denotes the Mumbai Region. This defines the physical location where your data is stored. 
5. **Permissions and Access :** By default, all S3 content is private. You control who can access your buckets and objects using permissions. These permissions can be managed through **IAM policies**, **bucket policies**, **Access Control Lists(ACLs),** or **pre-signed URLs** for temporary access.


I hosted a static website using an Amazon S3 bucket and deployed it globally via Amazon CloudFront. I created an S3 bucket to store the website files, configured it for static website hosting, and then set up a CloudFront distribution to serve the content with low latency. 

To securely grant CloudFront access to private S3 bucket, I created and attached an Origin Access Control(OAC), and updated the S3 bucket policy. After the distribution finished deploying, the website was successfully accessible through the CloudFront domain. 

Below is the screenshot of the distribution I created on CloudFront :
[![Screenshot-2025-06-01-222016.png](https://i.postimg.cc/T3T7pmtY/Screenshot-2025-06-01-222016.png)](https://postimg.cc/MvrbLckh)
Below is the screenshot of the Amazon S3 bucket I created :
[![Screenshot-2025-06-01-222003.png](https://i.postimg.cc/28Q9kTFK/Screenshot-2025-06-01-222003.png)](https://postimg.cc/KRYDQPWP)
Below is the screenshot of a file accessed on another tab :
[![Screenshot-2025-06-01-221950.png](https://i.postimg.cc/c185jdKZ/Screenshot-2025-06-01-221950.png)](https://postimg.cc/6Tt04JL1)
