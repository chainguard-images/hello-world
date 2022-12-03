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
| `latest` | `sha256:292ff82e31b95c82fc1f9e3df38da2a6e78ae047a7e7bf2e21c90d91e23eaa25`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:292ff82e31b95c82fc1f9e3df38da2a6e78ae047a7e7bf2e21c90d91e23eaa25) | `amd64` `arm64` `armv7` |



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
        "docker-manifest-digest": "sha256:292ff82e31b95c82fc1f9e3df38da2a6e78ae047a7e7bf2e21c90d91e23eaa25"
      },
      "type": "cosign container image signature"
    },
    "optional": {
      "1.3.6.1.4.1.57264.1.1": "https://token.actions.githubusercontent.com",
      "1.3.6.1.4.1.57264.1.2": "schedule",
      "1.3.6.1.4.1.57264.1.3": "468eb4291435a89b1ee2c56a2a1665f18a974bd6",
      "1.3.6.1.4.1.57264.1.4": "Create Release",
      "1.3.6.1.4.1.57264.1.5": "chainguard-images/hello-world",
      "1.3.6.1.4.1.57264.1.6": "refs/heads/main",
      "Bundle": {
        "SignedEntryTimestamp": "MEYCIQD5ySqJcjbE6YaCloAc1Jjl8IkNSnUXPQGPVtikQKq5UgIhAIkUuZaTS/s+R/Ex9TRTtQXcN0wIn06Rx1QBsjvV2jI4",
        "Payload": {
          "body": "eyJhcGlWZXJzaW9uIjoiMC4wLjEiLCJraW5kIjoiaGFzaGVkcmVrb3JkIiwic3BlYyI6eyJkYXRhIjp7Imhhc2giOnsiYWxnb3JpdGhtIjoic2hhMjU2IiwidmFsdWUiOiIxNDQ2ZmU2OWNiNjU2ZjMxMzU5YjcxYmEzNDQ4MWQ1YjA0YzdlNGZkNGMzNjM5Y2VmMWJlYjg0ZmY0MDFiMDQ2In19LCJzaWduYXR1cmUiOnsiY29udGVudCI6Ik1FWUNJUURGdVdBSzN6WUJVanBJLzVKNG5kbkFyTzJtbXVNSXNtYTlHMCtVcWh2ZWtnSWhBTWNDREZJYlpiSlZaYjNqVFd1a1RrS1U4dFA2MjF6YkxsUG9GQk1EbHZGTSIsInB1YmxpY0tleSI6eyJjb250ZW50IjoiTFMwdExTMUNSVWRKVGlCRFJWSlVTVVpKUTBGVVJTMHRMUzB0Q2sxSlNVUjBSRU5EUVhweFowRjNTVUpCWjBsVllXZHFhbEpCV2xoeU5uQjVNMk5KZWxOR1draFRWbnA1Y0U1VmQwTm5XVWxMYjFwSmVtb3dSVUYzVFhjS1RucEZWazFDVFVkQk1WVkZRMmhOVFdNeWJHNWpNMUoyWTIxVmRWcEhWakpOVWpSM1NFRlpSRlpSVVVSRmVGWjZZVmRrZW1SSE9YbGFVekZ3WW01U2JBcGpiVEZzV2tkc2FHUkhWWGRJYUdOT1RXcEplRTFxUVhwTlJFRjNUMVJOTlZkb1kwNU5ha2w0VFdwQmVrMUVRWGhQVkUwMVYycEJRVTFHYTNkRmQxbElDa3R2V2tsNmFqQkRRVkZaU1V0dldrbDZhakJFUVZGalJGRm5RVVV3UzBGSWVUTjROMDlUVFdKRFZsSklUamxFYkdock9VdDNURzFtVEhReUwwUkllRFVLYXpnemNrRjZNRkV3V2pkTmFuVnRUMHgwZGxFNVVHOW1NbE5ITjBoaWFtRXJURFZ3V2s0MllqSlBTREpGY2tKMlZuRlBRMEZzYTNkblowcFdUVUUwUndwQk1WVmtSSGRGUWk5M1VVVkJkMGxJWjBSQlZFSm5UbFpJVTFWRlJFUkJTMEpuWjNKQ1owVkdRbEZqUkVGNlFXUkNaMDVXU0ZFMFJVWm5VVlZFVWpSVENtZHlOa0ZEUXl0a1lreGxhMWxKZGxkSk0ybzJVR28wZDBoM1dVUldVakJxUWtKbmQwWnZRVlV6T1ZCd2VqRlphMFZhWWpWeFRtcHdTMFpYYVhocE5Ga0tXa1E0ZDJKUldVUldVakJTUVZGSUwwSkhUWGRaV1ZwbVlVaFNNR05JVFRaTWVUbHVZVmhTYjJSWFNYVlpNamwwVERKT2IxbFhiSFZhTTFab1kyMVJkQXBoVnpGb1dqSldla3d5YUd4aVIzaDJURmhrZG1OdGVHdE1lVFZ1WVZoU2IyUlhTWFprTWpsNVlUSmFjMkl6WkhwTU0wcHNZa2RXYUdNeVZYVmxWMFowQ21KRlFubGFWMXA2VERKb2JGbFhVbnBNTWpGb1lWYzBkMDlSV1V0TGQxbENRa0ZIUkhaNlFVSkJVVkZ5WVVoU01HTklUVFpNZVRrd1lqSjBiR0pwTldnS1dUTlNjR0l5TlhwTWJXUndaRWRvTVZsdVZucGFXRXBxWWpJMU1GcFhOVEJNYlU1MllsUkJWMEpuYjNKQ1owVkZRVmxQTDAxQlJVTkNRV2g2V1RKb2JBcGFTRlp6V2xSQk1rSm5iM0pDWjBWRlFWbFBMMDFCUlVSQ1EyY3dUbXBvYkZscVVYbFBWRVV3VFhwV2FFOUViR2xOVjFac1RXMU5NVTV0UlhsWlZFVXlDazVxVm0xTlZHaG9UMVJqTUZsdFVUSk5RbmRIUTJselIwRlJVVUpuTnpoM1FWRlJSVVJyVG5sYVYwWXdXbE5DVTFwWGVHeFpXRTVzVFVOelIwTnBjMGNLUVZGUlFtYzNPSGRCVVZWRlNGZE9iMWxYYkhWYU0xWm9ZMjFSZEdGWE1XaGFNbFo2VERKb2JHSkhlSFpNV0dSMlkyMTRhMDFDTUVkRGFYTkhRVkZSUWdwbk56aDNRVkZaUlVRelNteGFiazEyWVVkV2FGcElUWFppVjBad1ltcERRbWxSV1V0TGQxbENRa0ZJVjJWUlNVVkJaMUkzUWtoclFXUjNRakZCVGpBNUNrMUhja2Q0ZUVWNVdYaHJaVWhLYkc1T2QwdHBVMncyTkROcWVYUXZOR1ZMWTI5QmRrdGxOazlCUVVGQ2FFNVdVazVKU1VGQlFWRkVRVVZaZDFKQlNXY0tXaTlhYmtWWmVIUmtkRTlFTTBJMmNrSlNTVFpSSzNaSVNHWjJXWHByU21zdlRVMVJaek5KVTI5aFRVTkpSRTltY3pWWlRXRjFPWE52ZG1KM2VsQmliQXBRTlRoclVVaEdUVlY0VTJsU05ISm1WR1JPYkdsRE5YQk5RVzlIUTBOeFIxTk5ORGxDUVUxRVFUSm5RVTFIVlVOTlF6QmxVRVJMYjJwa0syZzRXRXBMQ2xOSFJHcFNUMVJrTDA5VlVHMVVOVlJqT1VWdVVHWnJjamhJYjJwR2FWcDJjeXR5TWpkaFR6VkVaSGhrVFV4VFpIVkJTWGhCVUhkNFEwSjRhSFpSWlVvS1lYTjZXbXhWUlhoblZUbG5WMjkyY25ZeEwyRndZa0ZaZEhFd2IxZHBVM1JpT1ZkRllrUlBMMk5DY1RnMmQzSndXVE42TmtoblBUMEtMUzB0TFMxRlRrUWdRMFZTVkVsR1NVTkJWRVV0TFMwdExRbz0ifX19fQ==",
          "integratedTime": 1670026187,
          "logIndex": 8325454,
          "logID": "c0d23d6ad406973f9559f3ba2d1ca01f84147d8ffc5b8445c224f98b9591801d"
        }
      },
      "Issuer": "https://token.actions.githubusercontent.com",
      "Subject": "https://github.com/chainguard-images/hello-world/.github/workflows/release.yaml@refs/heads/main",
      "githubWorkflowName": "Create Release",
      "githubWorkflowRef": "refs/heads/main",
      "githubWorkflowRepository": "chainguard-images/hello-world",
      "githubWorkflowSha": "468eb4291435a89b1ee2c56a2a1665f18a974bd6",
      "githubWorkflowTrigger": "schedule",
      "run_attempt": "1",
      "run_id": "3606000206",
      "sha": "468eb4291435a89b1ee2c56a2a1665f18a974bd6"
    }
  }
]
```

You can verify that the image was built in Github Actions in this repository from the `Issuer` and `Subject` fields.
</details>

## Build

This image is built with [melange](https://github.com/chainguard-dev/melange) and [apko](https://github.com/chainguard-dev/apko).

