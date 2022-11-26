# hello-world

<!---
Note: Do NOT edit directly, this file was generated using https://github.com/chainguard-images/readme-generator
-->

[![CI status](https://github.com/chainguard-images/hello-world/actions/workflows/release.yaml/badge.svg)](https://github.com/chainguard-images/hello-world/actions/workflows/release.yaml)

Hello, world!

## Get It!

The image is available on `cgr.dev`:

```
docker pull cgr.dev/chainguard/hello-world:latest
```

## Supported tags

| Tag | Digest | Arch |
| --- | ------ | ---- |
| `latest` | `sha256:eca2decc4809f0bca7e23d05226caebdf47058e9dfb259ab964dee70f5dd1e85`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:eca2decc4809f0bca7e23d05226caebdf47058e9dfb259ab964dee70f5dd1e85) | `amd64` `arm64` `armv7` |



## Signing

All Chainguard Images are signed using [Sigstore](https://sigstore.dev)!

<details>
<br/>
To verify the image, download <a href="https://github.com/sigstore/cosign">cosign</a> and run:

```
COSIGN_EXPERIMENTAL=1 cosign verify cgr.dev/chainguard/hello-world:latest | jq
```

Output:
```
Verification for cgr.dev/chainguard/hello-world:latest --
The following checks were performed on each of these signatures:
  - The cosign claims were validated
  - Existence of the claims in the transparency log was verified offline
  - Any certificates were verified against the Fulcio roots.
[
  {
    "critical": {
      "identity": {
        "docker-reference": "ghcr.io/chainguard-images/hello-world"
      },
      "image": {
        "docker-manifest-digest": "sha256:eca2decc4809f0bca7e23d05226caebdf47058e9dfb259ab964dee70f5dd1e85"
      },
      "type": "cosign container image signature"
    },
    "optional": {
      "1.3.6.1.4.1.57264.1.1": "https://token.actions.githubusercontent.com",
      "1.3.6.1.4.1.57264.1.2": "schedule",
      "1.3.6.1.4.1.57264.1.3": "3a9d7b20da7c1405be1d01c8418c442c8d97fa31",
      "1.3.6.1.4.1.57264.1.4": "Create Release",
      "1.3.6.1.4.1.57264.1.5": "chainguard-images/hello-world",
      "1.3.6.1.4.1.57264.1.6": "refs/heads/main",
      "Bundle": {
        "SignedEntryTimestamp": "MEUCIHwNbT/A4KmVx6rQMomU9iWpKWC8+0gKGBqO/aZUMIqhAiEAxDflW91RIxRPglwxbHeHZEYfkfLIu9KsPAttI5iVFuk=",
        "Payload": {
          "body": "eyJhcGlWZXJzaW9uIjoiMC4wLjEiLCJraW5kIjoiaGFzaGVkcmVrb3JkIiwic3BlYyI6eyJkYXRhIjp7Imhhc2giOnsiYWxnb3JpdGhtIjoic2hhMjU2IiwidmFsdWUiOiJlY2ViNjQ4YmI3YjhjM2Y4YjMxOGQ5NzcxM2MxMmI4NjU0OGQ0ZWVlYmJiOTYyMGRiMDNiYWJkYjNmMGZmNzg5In19LCJzaWduYXR1cmUiOnsiY29udGVudCI6Ik1FUUNJRGR5ZEJxNmlQY1JjSGh6ZTNJUFRsMitCQnlEdHlGRzIrSVhxQkI4NEtUMEFpQlIvV3JjN3Niek1JLytPTnNLeHU2Nm10cjdRVnI2TmRWRTVqMW1oOFJoUEE9PSIsInB1YmxpY0tleSI6eyJjb250ZW50IjoiTFMwdExTMUNSVWRKVGlCRFJWSlVTVVpKUTBGVVJTMHRMUzB0Q2sxSlNVUjBSRU5EUVhwMVowRjNTVUpCWjBsVlN5OHZjSGx2VDI5WFNuRlhZMDUwT1hoVGIxTktkVmgyVW1acmQwTm5XVWxMYjFwSmVtb3dSVUYzVFhjS1RucEZWazFDVFVkQk1WVkZRMmhOVFdNeWJHNWpNMUoyWTIxVmRWcEhWakpOVWpSM1NFRlpSRlpSVVVSRmVGWjZZVmRrZW1SSE9YbGFVekZ3WW01U2JBcGpiVEZzV2tkc2FHUkhWWGRJYUdOT1RXcEplRTFVU1RKTlJFRjRUVVJSZUZkb1kwNU5ha2w0VFZSSk1rMUVRWGxOUkZGNFYycEJRVTFHYTNkRmQxbElDa3R2V2tsNmFqQkRRVkZaU1V0dldrbDZhakJFUVZGalJGRm5RVVUwVDJwUFEyZHRPR04zVVdoVFV6QnRhR3BqUjNweVNEUXJXVUpLVkVoT1p6TnhiMHdLZFhGTGJGRndkSEJJZEZSU1pra3hTSFZDYkcxRWF6ZFRUWHB2Y2s5Q1QyWjFjVkJXUkdWNGFFTm9lakZLU0U5dVUyRlBRMEZzYjNkblowcFhUVUUwUndwQk1WVmtSSGRGUWk5M1VVVkJkMGxJWjBSQlZFSm5UbFpJVTFWRlJFUkJTMEpuWjNKQ1owVkdRbEZqUkVGNlFXUkNaMDVXU0ZFMFJVWm5VVlZqYWxWcENpOXBSR2hvTmxsNk1YSkdjMnBETmtNeWFtbDRjbTgwZDBoM1dVUldVakJxUWtKbmQwWnZRVlV6T1ZCd2VqRlphMFZhWWpWeFRtcHdTMFpYYVhocE5Ga0tXa1E0ZDJKUldVUldVakJTUVZGSUwwSkhUWGRaV1ZwbVlVaFNNR05JVFRaTWVUbHVZVmhTYjJSWFNYVlpNamwwVERKT2IxbFhiSFZhTTFab1kyMVJkQXBoVnpGb1dqSldla3d5YUd4aVIzaDJURmhrZG1OdGVHdE1lVFZ1WVZoU2IyUlhTWFprTWpsNVlUSmFjMkl6WkhwTU0wcHNZa2RXYUdNeVZYVmxWMFowQ21KRlFubGFWMXA2VERKb2JGbFhVbnBNTWpGb1lWYzBkMDlSV1V0TGQxbENRa0ZIUkhaNlFVSkJVVkZ5WVVoU01HTklUVFpNZVRrd1lqSjBiR0pwTldnS1dUTlNjR0l5TlhwTWJXUndaRWRvTVZsdVZucGFXRXBxWWpJMU1GcFhOVEJNYlU1MllsUkJWMEpuYjNKQ1owVkZRVmxQTDAxQlJVTkNRV2g2V1RKb2JBcGFTRlp6V2xSQk1rSm5iM0pDWjBWRlFWbFBMMDFCUlVSQ1EyZDZXVlJzYTA0eVNYbE5SMUpvVGpKTmVFNUVRVEZaYlZWNFdrUkJlRmw2WnpCTlZHaHFDazVFVVhsWmVtaHJUMVJrYlZsVVRYaE5RbmRIUTJselIwRlJVVUpuTnpoM1FWRlJSVVJyVG5sYVYwWXdXbE5DVTFwWGVHeFpXRTVzVFVOelIwTnBjMGNLUVZGUlFtYzNPSGRCVVZWRlNGZE9iMWxYYkhWYU0xWm9ZMjFSZEdGWE1XaGFNbFo2VERKb2JHSkhlSFpNV0dSMlkyMTRhMDFDTUVkRGFYTkhRVkZSUWdwbk56aDNRVkZaUlVRelNteGFiazEyWVVkV2FGcElUWFppVjBad1ltcERRbWxuV1V0TGQxbENRa0ZJVjJWUlNVVkJaMUk0UWtodlFXVkJRakpCVGpBNUNrMUhja2Q0ZUVWNVdYaHJaVWhLYkc1T2QwdHBVMncyTkROcWVYUXZOR1ZMWTI5QmRrdGxOazlCUVVGQ2FFeEdSbTg1VVVGQlFWRkVRVVZqZDFKUlNXZ0tRVXhzVWtKWFRERjBSMGxOTTBKSVVHdGhXSEk1VWs1elptSkdOaXRoY3pGbWVFdGlLM0V6YTNkSGIzVkJhVUZVY1ZSRGRrTXJZblJyUW5wUlJqaE9hUW8zYWxVMFYwWjNXbVl2Wm5WblpFbHJXRGxJVjNSNlVrTkpWRUZMUW1kbmNXaHJhazlRVVZGRVFYZE9ia0ZFUW10QmFrRlJOMmh0YTJGWlVtcEJNbmd3Q25WT01rcHViRVZqUlZsa2JYRjNhMFpEWWpaSVJHaElTbmRhZG5WTE1IUTVjRFY0YjBSNk9URnhUMGh4VmxRemNrMHlXVU5OUlc1TVZqVXlWSHBJTUdNS1N5OU9WVWhQTkdKT1dscG1lblpzVFZsdUt5c3hha3M0VURoTFdWcE9hbmRZVjBWbFNtaHZNMGx6TDJkSWEwb3JNR3hHTTAxUlBUMEtMUzB0TFMxRlRrUWdRMFZTVkVsR1NVTkJWRVV0TFMwdExRbz0ifX19fQ==",
          "integratedTime": 1669421449,
          "logIndex": 7856637,
          "logID": "c0d23d6ad406973f9559f3ba2d1ca01f84147d8ffc5b8445c224f98b9591801d"
        }
      },
      "Issuer": "https://token.actions.githubusercontent.com",
      "Subject": "https://github.com/chainguard-images/hello-world/.github/workflows/release.yaml@refs/heads/main",
      "githubWorkflowName": "Create Release",
      "githubWorkflowRef": "refs/heads/main",
      "githubWorkflowRepository": "chainguard-images/hello-world",
      "githubWorkflowSha": "3a9d7b20da7c1405be1d01c8418c442c8d97fa31",
      "githubWorkflowTrigger": "schedule",
      "run_attempt": "1",
      "run_id": "3551372839",
      "sha": "3a9d7b20da7c1405be1d01c8418c442c8d97fa31"
    }
  }
]
```

You can verify that the image was built in Github Actions in this repository from the `Issuer` and `Subject` fields.
</details>

## Build

This image is built with [melange](https://github.com/chainguard-dev/melange) and [apko](https://github.com/chainguard-dev/apko).

