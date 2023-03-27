# sast-snyk-check

sast-snyk-check task uses [Snyk Code](https://snyk.io/product/snyk-code/) tool to perform Static Application Security Testing (SAST) for [Snyk](https://snyk.io/), a popular cloud-native application security platform.

Snyk's SAST tool uses a combination of static analysis and machine learning techniques to scan an application's source code for potential security vulnerabilities, including common issues such as SQL injection, cross-site scripting (XSS), and code injection attacks.

This task is executed only if the user provides a Snyk token stored in a secret in their namespace. The name of the secret then needs to be supplied in the `snyk-secret` pipeline parameter.
