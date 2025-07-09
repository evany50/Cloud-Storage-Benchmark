# Cloud-Storage-Benchmark

## Overview
Benchmarks upload/download performance across multiple cloud storage providers:
- Backblaze B2
- Cloudflare R2 
- IBM Cloud Object Storage

Measures transfer speeds for different file sizes and generates comparative visualizations.

## Configuration
1. Edit the endpoint, bucket name, access key, secret key and region for each provider.
 ```python
   PROVIDERS = {
       'b2': {  # Backblaze B2
           'endpoint': 'https://s3.us-east-005.backblazeb2.com',  # Replace with your endpoint
           'bucket': 'your-bucket-name',                          # Your bucket name
           'access_key': 'your_key_id_here',                      # Your access key
           'secret_key': 'your_secret_key_here',                  # Your secret key
           'region': 'us-east-005'                                # Your bucket's region
       }
```
2. Install dependencies:
```bash
pip install "boto3==1.24.96" "botocore==1.27.96"
```
