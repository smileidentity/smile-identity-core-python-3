# Smile Identity Python Server Side Library

Smile Identity provides the best solutions for real time Digital KYC, identity verification, user onboarding, and user authentication across Africa. Our server side libraries make it easy to integrate us on the server-side. Since the library is server-side, you will be required to pass the images (if required) to the library.
If you haven’t already, sign up for a free Smile Identity account, which comes with Sandbox access.

## Features
The library exposes four classes namely; the WebApi class, the IDApi class, the Signature class, and the Utilities class.

The WebApi class has the following public methods:
- submit_job - handles submission of any Smile Identity products that requires an image i.e. [Biometric KYC](https://docs.smileidentity.com/products/biometric-identity-lookup), [Document Verification](https://docs.smileidentity.com/products/document-verification), and [SmartSelfie<sup>TM</sup> Authentication](https://docs.smileidentity.com/products/biometric-authentication).
- get_web_token - handles generation of web token, if you are using the [Hosted Web Integration](https://docs.smileidentity.com/web-mobile-web/web-integration-beta).

The IDApi class has the following public method:
- submit_job - handles submission of [Enhanced KYC](https://docs.smileidentity.com/products/identity-lookup) and [Basic KYC](https://docs.smileidentity.com/products/id-verification).

The Signature class has the following public methods:
- generate_signature - generate a signature which is then passed as a signature param when making requests to the Smile Identity server
- confirm_signature - ensure a response is truly from the Smile Identity server by confirming the incoming signature

The Utilities Class allows you as the Partner to have access to our general Utility functions to gain access to your data. It has the following public methods:
- get_job_status - retrieve information & results of a job. Read more on job status in the [Smile Identity documentation](https://docs.smileidentity.com/further-reading/job-status).
- get_smile_id_services - general information about different smile identity products such as required inputs for each supported id type.

## Dependencies
- Python 3

## Installation
`pip install smile-id-core`

## License
MIT License

## Documentation
For extensive instructions on usage of the library and sample codes, please refer to the official Smile Identity documentation https://docs.smileidentity.com/server-to-server/python.

## Getting Help
For usage questions, the best resource is our [official documentation](https://docs.smileidentity.com/). However, if you require further assistance, you can file a [support ticket via our portal](https://portal.smileidentity.com/partner/support/tickets) or visit the [contact us](https://www.smileidentity.com/contact-us/) page on our website.

## Contributing
Bug reports and pull requests are welcome on GitHub at https://github.com/smileidentity/smile-identity-core-python-3.
Please format the code with black prior to submitting pull requests, by running

`black .`