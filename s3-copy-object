
# Online Python - IDE, Editor, Compiler, Interpreter
import boto3

source_bucket = "source-bucket-nkm"
source_file = "1671905777033.jpg"

target_bucket = "target-bucket-nkm"
target_file = "1671905777033.jpg"

s3_client = boto3.client('s3')

try:
    # Copy the file from the source bucket to the destination bucket
    s3_client.copy_object(
        CopySource={"Bucket": source_bucket, "Key": source_file},
        Bucket=target_bucket,
        Key=target_file
    )
    print("File copied from {source_bucket}/{source_file} to {target_bucket}/{target_file}")
except Exception as e:
    print("An error occurred:", e)
