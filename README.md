This is a simple Docker container for [s3cmd](http://s3tools.org/s3cmd) : Command Line S3 Client and Backup for Linux and Mac.

Built using Alpine Linux as base image

Inspired by [samepage-labs/docker-s3cmd](https://github.com/samepage-labs/docker-s3cmd)

## Usage
Example usage:

`docker run flojon/s3cmd --access_key=S3_ACCESS_KEY --secret_key=S3_SECRET_KEY ls s3://bucket-name/`

If using alternative S3 provider you need to specify both --host and --host-bucket. Example for Digital Ocean Spaces (Amsterdam):

`docker run flojon/s3cmd --access_key=S3_ACCESS_KEY --secret_key=S3_SECRET_KEY --host=ams3.digitaloceanspaces.com --host-bucket="%(bucket)s.ams3.digitaloceanspaces.com" ls s3://bucket-name`

See [Usage](http://s3tools.org/usage) for full usage information.
