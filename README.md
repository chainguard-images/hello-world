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
| `latest` | `sha256:53def5c55e0e9cdd243e97f4a86b36a11e0e542e3c2b458c650b74e8ad1b8495`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:53def5c55e0e9cdd243e97f4a86b36a11e0e542e3c2b458c650b74e8ad1b8495) | `amd64` `arm64` `armv7` |



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
        "docker-manifest-digest": "sha256:53def5c55e0e9cdd243e97f4a86b36a11e0e542e3c2b458c650b74e8ad1b8495"
      },
      "type": "cosign container image signature"
    },
    "optional": {
      "1.3.6.1.4.1.57264.1.1": "https://token.actions.githubusercontent.com",
      "1.3.6.1.4.1.57264.1.2": "schedule",
      "1.3.6.1.4.1.57264.1.3": "153f0cc817122e089c67b68e865089905a4ec7a0",
      "1.3.6.1.4.1.57264.1.4": "Create Release",
      "1.3.6.1.4.1.57264.1.5": "chainguard-images/hello-world",
      "1.3.6.1.4.1.57264.1.6": "refs/heads/main",
      "Bundle": {
        "SignedEntryTimestamp": "MEUCIQDg/n56WPlMMr6dQwC1DgN1vmEKNUzhEDKFAM1jBGt+cwIgNJlHpMXTPNdTj+VFc7X4hjJ22GN29b6Vkb6nqEzxe0Y=",
        "Payload": {
          "body": "eyJhcGlWZXJzaW9uIjoiMC4wLjEiLCJraW5kIjoiaGFzaGVkcmVrb3JkIiwic3BlYyI6eyJkYXRhIjp7Imhhc2giOnsiYWxnb3JpdGhtIjoic2hhMjU2IiwidmFsdWUiOiJjMjdhYWFhMjVmYWE4NWRmZTFjYjUyOTc2OTZiNGQxNzEzN2Y1OGMyYzE2NGFmNzdhZTA2MjNlZmVmNWU2OGQ4In19LCJzaWduYXR1cmUiOnsiY29udGVudCI6Ik1FUUNJRTZFOWxpVGF6aDIzc055OWx4dncrQmw3blQ5VEZZK3VHVmRFbUhXNitMSkFpQkV3QmlOSzZOMlZLUjlGZ2Q0azcxdmNhQkdBZXZqQ3hvYVNJRXpKK3VBdUE9PSIsInB1YmxpY0tleSI6eyJjb250ZW50IjoiTFMwdExTMUNSVWRKVGlCRFJWSlVTVVpKUTBGVVJTMHRMUzB0Q2sxSlNVUjBSRU5EUVhweFowRjNTVUpCWjBsVlR5OTBNRzVtU0RCNlF6UlpkVFF2VFRWYVpGSXZZMFZJYWtwVmQwTm5XVWxMYjFwSmVtb3dSVUYzVFhjS1RucEZWazFDVFVkQk1WVkZRMmhOVFdNeWJHNWpNMUoyWTIxVmRWcEhWakpOVWpSM1NFRlpSRlpSVVVSRmVGWjZZVmRrZW1SSE9YbGFVekZ3WW01U2JBcGpiVEZzV2tkc2FHUkhWWGRJYUdOT1RXcEplRTFVUlRSTlJFVjNUMVJKZUZkb1kwNU5ha2w0VFZSRk5FMUVSWGhQVkVsNFYycEJRVTFHYTNkRmQxbElDa3R2V2tsNmFqQkRRVkZaU1V0dldrbDZhakJFUVZGalJGRm5RVVZTTDBoeFpqTjRMMmhwZDJWdmFHdEdkMGR0Ulc4dkwxRnlVamxVTjFGUVlsUXdVazBLTnpSRk0zTTVSWFpzVDA5ak5tZHhlbE5DYjFONE9WUktOVTlqVldNM2FVRm1OMEptZW1SUlMxUjFOblk0TUZSNlJtRlBRMEZzYTNkblowcFdUVUUwUndwQk1WVmtSSGRGUWk5M1VVVkJkMGxJWjBSQlZFSm5UbFpJVTFWRlJFUkJTMEpuWjNKQ1owVkdRbEZqUkVGNlFXUkNaMDVXU0ZFMFJVWm5VVlU0VWtoR0NsZzRRM1ZQV214NFlVVnRjVEJEUWxocFdqVTJWRkJWZDBoM1dVUldVakJxUWtKbmQwWnZRVlV6T1ZCd2VqRlphMFZhWWpWeFRtcHdTMFpYYVhocE5Ga0tXa1E0ZDJKUldVUldVakJTUVZGSUwwSkhUWGRaV1ZwbVlVaFNNR05JVFRaTWVUbHVZVmhTYjJSWFNYVlpNamwwVERKT2IxbFhiSFZhTTFab1kyMVJkQXBoVnpGb1dqSldla3d5YUd4aVIzaDJURmhrZG1OdGVHdE1lVFZ1WVZoU2IyUlhTWFprTWpsNVlUSmFjMkl6WkhwTU0wcHNZa2RXYUdNeVZYVmxWMFowQ21KRlFubGFWMXA2VERKb2JGbFhVbnBNTWpGb1lWYzBkMDlSV1V0TGQxbENRa0ZIUkhaNlFVSkJVVkZ5WVVoU01HTklUVFpNZVRrd1lqSjBiR0pwTldnS1dUTlNjR0l5TlhwTWJXUndaRWRvTVZsdVZucGFXRXBxWWpJMU1GcFhOVEJNYlU1MllsUkJWMEpuYjNKQ1owVkZRVmxQTDAxQlJVTkNRV2g2V1RKb2JBcGFTRlp6V2xSQk1rSm5iM0pDWjBWRlFWbFBMMDFCUlVSQ1EyZDRUbFJPYlUxSFRtcFBSRVV6VFZSSmVWcFVRVFJQVjAweVRqSkpNazlIVlRST2FsVjNDazlFYXpWTlJGWm9Ua2RXYWs0eVJYZE5RbmRIUTJselIwRlJVVUpuTnpoM1FWRlJSVVJyVG5sYVYwWXdXbE5DVTFwWGVHeFpXRTVzVFVOelIwTnBjMGNLUVZGUlFtYzNPSGRCVVZWRlNGZE9iMWxYYkhWYU0xWm9ZMjFSZEdGWE1XaGFNbFo2VERKb2JHSkhlSFpNV0dSMlkyMTRhMDFDTUVkRGFYTkhRVkZSUWdwbk56aDNRVkZaUlVRelNteGFiazEyWVVkV2FGcElUWFppVjBad1ltcERRbWxSV1V0TGQxbENRa0ZJVjJWUlNVVkJaMUkzUWtoclFXUjNRakZCVGpBNUNrMUhja2Q0ZUVWNVdYaHJaVWhLYkc1T2QwdHBVMncyTkROcWVYUXZOR1ZMWTI5QmRrdGxOazlCUVVGQ2FFbG9TV1JwYzBGQlFWRkVRVVZaZDFKQlNXY0tVMmhOU3pFdlYwTnVaQzgxU0c1ME9VdHVSV2R1YkVaNGMwb3lZVXBVUVZBM1dVYzNLMmt2VEZkcVFVTkpRa2hoZUdWUlRtNUxhVzVUY3psNVNXaHJMd28yUkVGcVJFaEhNakEyVTFGVlZITkVaRkptUkZGS2JXbE5RVzlIUTBOeFIxTk5ORGxDUVUxRVFUSm5RVTFIVlVOTlVVUnpRV1EyYkRoclVYRkRiamRsQ2taSVdGZE9iREl6UmxoUGJuUnRTM2gzTWpKYU9GUmxLMWMwT1ZwcWVUQnBaVzVEYzNsdVlsUlpjV2x4V0ZaMlFVVjBjME5OUmxsWU5WUlVPVkJJYld3S2NHWlVZVk4zYldSdlVFOUpiRXcxWlZkRVZ6QTJORkJwVTBneFJYVXpWaXQ0TkhGdlNUSm1PU3RWYVZGVUszaGFOMW8ySzFsUlBUMEtMUzB0TFMxRlRrUWdRMFZTVkVsR1NVTkJWRVV0TFMwdExRbz0ifX19fQ==",
          "integratedTime": 1668733769,
          "logIndex": 7310656,
          "logID": "c0d23d6ad406973f9559f3ba2d1ca01f84147d8ffc5b8445c224f98b9591801d"
        }
      },
      "Issuer": "https://token.actions.githubusercontent.com",
      "Subject": "https://github.com/chainguard-images/hello-world/.github/workflows/release.yaml@refs/heads/main",
      "githubWorkflowName": "Create Release",
      "githubWorkflowRef": "refs/heads/main",
      "githubWorkflowRepository": "chainguard-images/hello-world",
      "githubWorkflowSha": "153f0cc817122e089c67b68e865089905a4ec7a0",
      "githubWorkflowTrigger": "schedule",
      "run_attempt": "1",
      "run_id": "3493323438",
      "sha": "153f0cc817122e089c67b68e865089905a4ec7a0"
    }
  }
]
```

You can verify that the image was built in Github Actions in this repository from the `Issuer` and `Subject` fields.
</details>

## Build

This image is built with [melange](https://github.com/chainguard-dev/melange) and [apko](https://github.com/chainguard-dev/apko).

