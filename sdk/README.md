# AWS EC2 FPGA Software Development Kit

This directory includes the drivers and runtime environment required by any EC2 Instance running on F1. It includes the drivers and tools to interact with pre-built AFIs that are loaded to EC2 F1 FPGAs.

The [SDK management directory](./management) contains the [Amazon FPGA Image (AFI) Management Tools](./management/fpga_image_tools/README.md), which includes both the source code to the AFI Management Tools as well as detailed [descriptions of the commands](./management/fpga_image_tools/README.md) to use on an F1 instance.

The SDK is **NOT** used to build or register AFI, rather it is only used for managing and deploying pre-built AFIs. For building and registering AFIs, please refer to the [HDK](../hdk/README.md).

**NOTE:** This SDK is designed and testing for Linux environments only.

# Quick Start

## Using an AFI on EC2 F1

You can setup and install the SDK with the following few steps.  Note that the first two steps may be skipped if you have already ran them in the above HDK setup.

    $ git clone https://github.com/aws/aws-fpga   # Fetch the HDK and SDK code
    $ cd aws-fpga                                 # Move to the root directory of the repository before running the next script
    $ source sdk_setup.sh                         # Set up the envronment variables, build and install the SDK
