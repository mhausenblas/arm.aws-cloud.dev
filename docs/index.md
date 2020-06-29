This site is dedicated to documenting resources on the topic of using [Arm architecture](https://en.wikipedia.org/wiki/ARM_architecture)-based systems on AWS.

!!! note
    If you are new to Arm, consider perusing the official [docs](https://developer.arm.com/docs) where you can
    download a range of hardware and software-related background information.

## Instances

AWS offers a number of options to run apps on Arm architecture-based EC2 instances:

- The first-generation [Graviton](https://aws.amazon.com/ec2/graviton/) A1 instances launched in 2018:
    - [Getting started with the A1 instance](https://aws.amazon.com/blogs/compute/getting-started-with-the-a1-instance/)
    - [AWS Designed Processor: Graviton](https://perspectives.mvdirona.com/2018/11/aws-designed-processor-graviton/) by James Hamilton
- The Graviton2 instances launched in 2019:
    - Check out the AWS re:Invent 2019 session "[Deep dive on Arm-based EC2 instances powered by AWS Graviton](https://www.youtube.com/watch?v=4jImmuMqnwc)" (CMP322-R1).
    - Read about the new instance family and how to get preview access in Jeff Barr's blog post [Coming Soon – Graviton2-Powered General Purpose, Compute-Optimized, & Memory-Optimized EC2 Instances](https://aws.amazon.com/blogs/aws/coming-soon-graviton2-powered-general-purpose-compute-optimized-memory-optimized-ec2-instances/).

## Containers

For cloud native applications, you can use containers:

- Learn about how to [get started with Docker on Arm](https://community.arm.com/developer/tools-software/tools/b/tools-software-ides-blog/posts/getting-started-with-docker-on-arm).
- If you want to package and distribute your apps, have a look at [cross building Arm images on Docker Desktop](https://medium.com/@carlosedp/cross-building-arm64-images-on-docker-desktop-254d1e0bc1f9).
- Manually follow the steps described in [Arm Support in Amazon EKS](https://docs.aws.amazon.com/eks/latest/userguide/arm-support.html) or use a script [for provisioning an EKS cluster](https://gist.github.com/mhausenblas/a1d195745267811b68055320f9844fe1) using `eksctl`.

## Devices

For IoT and/or hybrid use cases:

- Learn how to set up a [Raspberry Pi for AWS IoT Greengrass](https://docs.aws.amazon.com/greengrass/latest/developerguide/setup-filter.rpi.html)
- Check out these AWS re:Invent sessions:
    - "[Computing at the Edge with AWS Greengrass & Amazon FreeRTOS](https://www.youtube.com/watch?v=MXEBjUZtT8Y)" (IOT206), 2018
    - "[Amazon FreeRTOS: IoT Operating System for Microcontrollers](https://www.youtube.com/watch?v=7fNFKYAuHls)" (IOT208), 2018
