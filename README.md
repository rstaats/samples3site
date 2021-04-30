This is a sample project page to demonstrate using Amazon S3 as a web hosting solution for a static site. 


#### Bucket Policy:

Below is the bucket polciy we will be using to allow our S3 bucket objects to be accessible. Be sure to change Bucket-Name to match the name of your bucket in the policy below:

```
{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Sid": "PublicReadGetObject",
            "Effect": "Allow",
            "Principal": "*",
            "Action": [
                "s3:GetObject"
            ],
            "Resource": [
                "arn:aws:s3:::Bucket-Name/*"
            ]
        }
    ]
}

```


#### Credits:

	Background Image:
		Ryan Schroeder via Unsplash (unsplash.com - CC0 licensed)
			"Icefields" (flickr.com/photos/ryanschroeder/11876741703)

	Icons:
		Font Awesome (fontawesome.io)

	Other:
		Responsive Tools (github.com/ajlkn/responsive-tools)
