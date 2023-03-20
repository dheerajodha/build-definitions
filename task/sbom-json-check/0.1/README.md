# sbom-json-check task

## Description:

sbom-json-check task verifies the integrity and security of a [Software Bill of Materials](https://www.cisa.gov/sbom) (SBOM) file in JSON format. [Refer to this article](https://www.redhat.com/en/blog/how-red-hat-addressing-demand-develop-offerings-more-securely) to learn more about SBOM.

This task checks the syntax of the sbom-cyclonedx.json file (found in the `/root/buildinfo/content_manifests/` directory) using the [CyloneDX](https://cyclonedx.org/) tool. This tool is being led by longtime security community leader Open Web Application Security Project ([OWASP](https://owasp.org/)). CycloneDX is a self-defined “lightweight SBOM standard designed for use in application security contexts and supply chain component analysis.”

## Params:

| name         | description                           |
|--------------|---------------------------------------|
| IMAGE_URL    | Fully qualified image name to verify. |
| IMAGE_DIGEST | Image digest.                         |

## Results:

| name                  | description              |
|-----------------------|--------------------------|
| HACBS_TEST_OUTPUT     | Tekton task test output. |
