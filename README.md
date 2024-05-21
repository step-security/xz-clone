# Analysis of the Backdoored XZ Utils Build Process with Harden-Runner

The code was originally sourced from [Debian's repository](https://salsa.debian.org/debian/xz-utils/-/tree/debian/5.6.0-0.2?ref_type=tags), specifically the debian/5.6.0-0.2 tag.

The GitHub Actions workflow used to run the steps is configured to perform the following:
- Checkout the code from the repository
- Run the configure script to generate the Makefile
- Execute the make step to build the XZ Utils binary

The workflow integrates [Harden Runner](https://github.com/step-security/harden-runner) to monitor and analyze the build process. Here are the Harden Runner insights from the workflow execution:
https://app.stepsecurity.io/github/step-security/xz-clone/actions/runs/9102857670?jobid=25085154668&tab=file-events  

You can read the blog post here for more details:
https://www.stepsecurity.io/blog/analysis-of-backdoored-xz-utils-build-process-with-harden-runner
