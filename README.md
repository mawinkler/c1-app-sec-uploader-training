# Cloud One Application Security with PHP Uploader

This demo app for Cloud One Application Security create an Apache PHP based front end allowing to upload kind of files. It is to simulate file uploading capabilities from real world web applications.

Application Security integration done via the provided Dockerfile.

## Usage

First, clone the repo

Then build and run the container

```sh
# Build the image
docker build -t uploader .

# Run the container
docker run \
  --rm -p 80:80 \
  --name uploader \
  -e TREND_AP_KEY=<YOUR APP SEC GROUP KEY>
  -e TREND_AP_SECRET=<YOUR APP SEC GROUP SECRET>
  uploader
```

The upload app is accessible on port 80.

Finally, upload malicious files.

## Jenkins

An example Jenkins pipeline is provided to integrate this app to your Jenkins instance.

## Support

This is an Open Source community project. Project contributors may be able to help, depending on their time and availability. Please be specific about what you're trying to do, your system, and steps to reproduce the problem.

For bug reports or feature requests, please [open an issue](../../issues). You are welcome to [contribute](#contribute).

Official support from Trend Micro is not available. Individual contributors may be Trend Micro employees, but are not official support.

## Contribute

I do accept contributions from the community. To submit changes:

1. Fork this repository.
1. Create a new feature branch.
1. Make your changes.
1. Submit a pull request with an explanation of your changes or additions.

I will review and work with you to release the code.
