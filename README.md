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
| `latest` | `sha256:4541670dffa65eedda9e72871a2b6a6ee1a377ebe32dd9c48a684ac530586586`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:4541670dffa65eedda9e72871a2b6a6ee1a377ebe32dd9c48a684ac530586586) | `amd64` `arm64` `armv7` |



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
        "docker-manifest-digest": "sha256:4541670dffa65eedda9e72871a2b6a6ee1a377ebe32dd9c48a684ac530586586"
      },
      "type": "cosign container image signature"
    },
    "optional": {
      "1.3.6.1.4.1.57264.1.1": "https://token.actions.githubusercontent.com",
      "1.3.6.1.4.1.57264.1.2": "schedule",
      "1.3.6.1.4.1.57264.1.3": "8b8937b5d1273c9e4320537458bc8d0733582edc",
      "1.3.6.1.4.1.57264.1.4": "Create Release",
      "1.3.6.1.4.1.57264.1.5": "chainguard-images/hello-world",
      "1.3.6.1.4.1.57264.1.6": "refs/heads/main",
      "Bundle": {
        "SignedEntryTimestamp": "MEQCICe4M7hQUfPjE0HwbxBUG4w51Gyh0fpMWK4lu4qSeQ1KAiBMpYgV9SMmEiCdGUv/aF8vewuGwOCGwwbDIm5szCH8Yw==",
        "Payload": {
          "body": "eyJhcGlWZXJzaW9uIjoiMC4wLjEiLCJraW5kIjoiaGFzaGVkcmVrb3JkIiwic3BlYyI6eyJkYXRhIjp7Imhhc2giOnsiYWxnb3JpdGhtIjoic2hhMjU2IiwidmFsdWUiOiI3ZDU4MmY4NGFjZGRmODU5ZjcxYWMwZWU5Nzg4ZDQ3MWI0Y2Q1MzM3Y2MwZGY0OTU2NzNlMmY2NjNkYjc5ZTI1In19LCJzaWduYXR1cmUiOnsiY29udGVudCI6Ik1FVUNJQlQzYjRIRTdnNnl1L2s5ZDBBV3l0eWt6dUZ2MGNBRE5HU0JEQmpLbjJ3cEFpRUE4czkzSFBLMzZaaEltUDVPRHNlb1dtN3kzV1dtQll6U1BvWVBodjdhMlYwPSIsInB1YmxpY0tleSI6eyJjb250ZW50IjoiTFMwdExTMUNSVWRKVGlCRFJWSlVTVVpKUTBGVVJTMHRMUzB0Q2sxSlNVUjBla05EUVhwNVowRjNTVUpCWjBsVlIyVXdXVnBZTUZJelRDdENLekJuYW1abVpIUlpVR2d6VVhkM2QwTm5XVWxMYjFwSmVtb3dSVUYzVFhjS1RucEZWazFDVFVkQk1WVkZRMmhOVFdNeWJHNWpNMUoyWTIxVmRWcEhWakpOVWpSM1NFRlpSRlpSVVVSRmVGWjZZVmRrZW1SSE9YbGFVekZ3WW01U2JBcGpiVEZzV2tkc2FHUkhWWGRJYUdOT1RXcEplRTFVUlRWTlJFVjNUbXBKTTFkb1kwNU5ha2w0VFZSRk5VMUVSWGhPYWtrelYycEJRVTFHYTNkRmQxbElDa3R2V2tsNmFqQkRRVkZaU1V0dldrbDZhakJFUVZGalJGRm5RVVYwYzNKU2NFNVdNWFZ3WkhkNE1WWlVSRE5aV1M5SFprMWhVV3c1YUZabVlUQXZURkFLUzNKWFNWcFpUMFpTWTFGa1pFUTBaR0ZvU3pocGVHcE9jbTR3YmxWbmRraFFla0owUVZRck4xRnRia3B1U20xRFQwdFBRMEZzYzNkblowcFlUVUUwUndwQk1WVmtSSGRGUWk5M1VVVkJkMGxJWjBSQlZFSm5UbFpJVTFWRlJFUkJTMEpuWjNKQ1owVkdRbEZqUkVGNlFXUkNaMDVXU0ZFMFJVWm5VVlZpTkZOVUNrczBiekpUUkdScGRHMXFTWFZvTWtWSWFGVXhWRTFaZDBoM1dVUldVakJxUWtKbmQwWnZRVlV6T1ZCd2VqRlphMFZhWWpWeFRtcHdTMFpYYVhocE5Ga0tXa1E0ZDJKUldVUldVakJTUVZGSUwwSkhUWGRaV1ZwbVlVaFNNR05JVFRaTWVUbHVZVmhTYjJSWFNYVlpNamwwVERKT2IxbFhiSFZhTTFab1kyMVJkQXBoVnpGb1dqSldla3d5YUd4aVIzaDJURmhrZG1OdGVHdE1lVFZ1WVZoU2IyUlhTWFprTWpsNVlUSmFjMkl6WkhwTU0wcHNZa2RXYUdNeVZYVmxWMFowQ21KRlFubGFWMXA2VERKb2JGbFhVbnBNTWpGb1lWYzBkMDlSV1V0TGQxbENRa0ZIUkhaNlFVSkJVVkZ5WVVoU01HTklUVFpNZVRrd1lqSjBiR0pwTldnS1dUTlNjR0l5TlhwTWJXUndaRWRvTVZsdVZucGFXRXBxWWpJMU1GcFhOVEJNYlU1MllsUkJWMEpuYjNKQ1owVkZRVmxQTDAxQlJVTkNRV2g2V1RKb2JBcGFTRlp6V2xSQk1rSm5iM0pDWjBWRlFWbFBMMDFCUlVSQ1EyYzBXV3BuTlUxNlpHbE9WMUY0VFdwamVsbDZiR3hPUkUxNVRVUlZlazU2VVRGUFIwcHFDazlIVVhkT2VrMTZUbFJuZVZwWFVtcE5RbmRIUTJselIwRlJVVUpuTnpoM1FWRlJSVVJyVG5sYVYwWXdXbE5DVTFwWGVHeFpXRTVzVFVOelIwTnBjMGNLUVZGUlFtYzNPSGRCVVZWRlNGZE9iMWxYYkhWYU0xWm9ZMjFSZEdGWE1XaGFNbFo2VERKb2JHSkhlSFpNV0dSMlkyMTRhMDFDTUVkRGFYTkhRVkZSUWdwbk56aDNRVkZaUlVRelNteGFiazEyWVVkV2FGcElUWFppVjBad1ltcERRbWwzV1V0TGQxbENRa0ZJVjJWUlNVVkJaMUk1UWtoelFXVlJRak5CVGpBNUNrMUhja2Q0ZUVWNVdYaHJaVWhLYkc1T2QwdHBVMncyTkROcWVYUXZOR1ZMWTI5QmRrdGxOazlCUVVGQ2FFa3hjMHhYUlVGQlFWRkVRVVZuZDFKblNXZ0tRVXMzYW14QmJXMTZSM0E1Y2xOd2JqSkphV2QxVTNSd1NIQnNkbVEyVkVoWFVtWlNOMjlqVEhwdlRXMUJhVVZCTkRKQ1VEaHNORVk0VUhOd1NYZFFkZ3ByU2paQ1VtVjVVelJYV2t0aVVWZ3lSR3gxVFdSVlRqaDJjRmwzUTJkWlNVdHZXa2w2YWpCRlFYZE5SR0ZSUVhkYVowbDRRVWx6UWxKWVEySlpWMlpwQ2pWcGIxRmpZMEZyTnpOUE5YUnZNREpXWlRKRVJVUkxjekpoTUdwb1IwdHBibEZCYjNJdlRYSnVaVEJsTVUxVGJWZ3JSMVJ3WjBsNFFVdHRjbVpPVVZNS1NFRjFRVU1yVFZsdVRtTm5Zak1yVmpSNWNEZFBOM042VlhGeUwyeHNMMGRDTUhkcFQybzJaakl6TkN0SWQxVjNaM05FZG10d1NHMW1aejA5Q2kwdExTMHRSVTVFSUVORlVsUkpSa2xEUVZSRkxTMHRMUzBLIn19fX0=",
          "integratedTime": 1668819995,
          "logIndex": 7383491,
          "logID": "c0d23d6ad406973f9559f3ba2d1ca01f84147d8ffc5b8445c224f98b9591801d"
        }
      },
      "Issuer": "https://token.actions.githubusercontent.com",
      "Subject": "https://github.com/chainguard-images/hello-world/.github/workflows/release.yaml@refs/heads/main",
      "githubWorkflowName": "Create Release",
      "githubWorkflowRef": "refs/heads/main",
      "githubWorkflowRepository": "chainguard-images/hello-world",
      "githubWorkflowSha": "8b8937b5d1273c9e4320537458bc8d0733582edc",
      "githubWorkflowTrigger": "schedule",
      "run_attempt": "1",
      "run_id": "3501364167",
      "sha": "8b8937b5d1273c9e4320537458bc8d0733582edc"
    }
  }
]
```

You can verify that the image was built in Github Actions in this repository from the `Issuer` and `Subject` fields.
</details>

## Build

This image is built with [melange](https://github.com/chainguard-dev/melange) and [apko](https://github.com/chainguard-dev/apko).

