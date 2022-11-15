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
| `latest` | `sha256:ad2342fcd361861763c0703b205ee68d2e44f211436d724c48b83840ca5e97dd`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:ad2342fcd361861763c0703b205ee68d2e44f211436d724c48b83840ca5e97dd) | `amd64` `arm64` `armv7` |



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
        "docker-manifest-digest": "sha256:ad2342fcd361861763c0703b205ee68d2e44f211436d724c48b83840ca5e97dd"
      },
      "type": "cosign container image signature"
    },
    "optional": {
      "1.3.6.1.4.1.57264.1.1": "https://token.actions.githubusercontent.com",
      "1.3.6.1.4.1.57264.1.2": "schedule",
      "1.3.6.1.4.1.57264.1.3": "6bec98f9e6461695fea1cbba7f1902e148aa221b",
      "1.3.6.1.4.1.57264.1.4": "Create Release",
      "1.3.6.1.4.1.57264.1.5": "chainguard-images/hello-world",
      "1.3.6.1.4.1.57264.1.6": "refs/heads/main",
      "Bundle": {
        "SignedEntryTimestamp": "MEQCIGlK4H/StWmEe/hmOQPH1Nuj+8ZEmCGX2eB68S94idEmAiBkMNt60kgSSALo85D9Kh2p/7ulDJ4GyGpPPL+UnnNVZQ==",
        "Payload": {
          "body": "eyJhcGlWZXJzaW9uIjoiMC4wLjEiLCJraW5kIjoiaGFzaGVkcmVrb3JkIiwic3BlYyI6eyJkYXRhIjp7Imhhc2giOnsiYWxnb3JpdGhtIjoic2hhMjU2IiwidmFsdWUiOiI2YzhlN2FkOGMzYzI5MjUxMDU4ZGE4NzQwNGRiYjcyYzlmZGEzZDZiMTlhYTVhNjA2NTg4NDQ2NzMyYjIzMjRmIn19LCJzaWduYXR1cmUiOnsiY29udGVudCI6Ik1FVUNJUURMdVZWSk5iWVI5dkJvT1g2WVBYQXJkYkZJLy9hK2ZOWE9HeWJLYjlsZmhRSWdNS21WbFN1MXVkRy9QdVBCVkEwMEdpZjJ3bUx5ZTlIamlXTHYyaExzV3NnPSIsInB1YmxpY0tleSI6eyJjb250ZW50IjoiTFMwdExTMUNSVWRKVGlCRFJWSlVTVVpKUTBGVVJTMHRMUzB0Q2sxSlNVUjBha05EUVhwNVowRjNTVUpCWjBsVlVIVnRTMjFHVW5Jd2QwaEhLMVI1WVc5VU15dElTa2haZW1oRmQwTm5XVWxMYjFwSmVtb3dSVUYzVFhjS1RucEZWazFDVFVkQk1WVkZRMmhOVFdNeWJHNWpNMUoyWTIxVmRWcEhWakpOVWpSM1NFRlpSRlpSVVVSRmVGWjZZVmRrZW1SSE9YbGFVekZ3WW01U2JBcGpiVEZzV2tkc2FHUkhWWGRJYUdOT1RXcEplRTFVUlRGTlJFVjNUbFJWZVZkb1kwNU5ha2w0VFZSRk1VMUVSWGhPVkZWNVYycEJRVTFHYTNkRmQxbElDa3R2V2tsNmFqQkRRVkZaU1V0dldrbDZhakJFUVZGalJGRm5RVVUyZEVSQ2VDdGtkREZvZURWQmJEUndkekprZERSaE0wRkpVRFkyV1c5emJreG1TSEVLTUZaTWEyeG9ORVowVFRkQlFsVkdORFF4TUdOTkwweFVaV1UyYUdoRlRtd3JVREl4TVhSd2NsQXhRbGxDU2pKc1MyRlBRMEZzYzNkblowcFlUVUUwUndwQk1WVmtSSGRGUWk5M1VVVkJkMGxJWjBSQlZFSm5UbFpJVTFWRlJFUkJTMEpuWjNKQ1owVkdRbEZqUkVGNlFXUkNaMDVXU0ZFMFJVWm5VVlZoV0RGMkNpczFWbXN5VVVwM1p6WktZbkJLY0RGdk0wSkJOVFF3ZDBoM1dVUldVakJxUWtKbmQwWnZRVlV6T1ZCd2VqRlphMFZhWWpWeFRtcHdTMFpYYVhocE5Ga0tXa1E0ZDJKUldVUldVakJTUVZGSUwwSkhUWGRaV1ZwbVlVaFNNR05JVFRaTWVUbHVZVmhTYjJSWFNYVlpNamwwVERKT2IxbFhiSFZhTTFab1kyMVJkQXBoVnpGb1dqSldla3d5YUd4aVIzaDJURmhrZG1OdGVHdE1lVFZ1WVZoU2IyUlhTWFprTWpsNVlUSmFjMkl6WkhwTU0wcHNZa2RXYUdNeVZYVmxWMFowQ21KRlFubGFWMXA2VERKb2JGbFhVbnBNTWpGb1lWYzBkMDlSV1V0TGQxbENRa0ZIUkhaNlFVSkJVVkZ5WVVoU01HTklUVFpNZVRrd1lqSjBiR0pwTldnS1dUTlNjR0l5TlhwTWJXUndaRWRvTVZsdVZucGFXRXBxWWpJMU1GcFhOVEJNYlU1MllsUkJWMEpuYjNKQ1owVkZRVmxQTDAxQlJVTkNRV2g2V1RKb2JBcGFTRlp6V2xSQk1rSm5iM0pDWjBWRlFWbFBMMDFCUlVSQ1EyY3lXVzFXYWs5VWFHMVBWMVV5VGtSWmVFNXFhekZhYlZab1RWZE9hVmx0UlROYWFrVTFDazFFU214TlZGRTBXVmRGZVUxcVJtbE5RbmRIUTJselIwRlJVVUpuTnpoM1FWRlJSVVJyVG5sYVYwWXdXbE5DVTFwWGVHeFpXRTVzVFVOelIwTnBjMGNLUVZGUlFtYzNPSGRCVVZWRlNGZE9iMWxYYkhWYU0xWm9ZMjFSZEdGWE1XaGFNbFo2VERKb2JHSkhlSFpNV0dSMlkyMTRhMDFDTUVkRGFYTkhRVkZSUWdwbk56aDNRVkZaUlVRelNteGFiazEyWVVkV2FGcElUWFppVjBad1ltcERRbWwzV1V0TGQxbENRa0ZJVjJWUlNVVkJaMUk1UWtoelFXVlJRak5CVGpBNUNrMUhja2Q0ZUVWNVdYaHJaVWhLYkc1T2QwdHBVMncyTkROcWVYUXZOR1ZMWTI5QmRrdGxOazlCUVVGQ2FFaHFVMDVKUVVGQlFWRkVRVVZuZDFKblNXZ0tRVTFpWVd0a1owdDVORXRWVUU1MGFIVk1OVzFUVVVwaFZqaEtVVzVsWlZCcWVHVndlQzlVYWk4NWJGVkJhVVZCZWpNNGJHZFdjR1paTm5kMlQxWjFlQW96UkRCS09GbG5XblIyUVhScmJubG1kamxLVkZSS1lrYzNlR2QzUTJkWlNVdHZXa2w2YWpCRlFYZE5SR0ZCUVhkYVVVbDRRVTFqY2s5R2R6UjVLekJ3Q2xOb1kzZHdhVXBwUkdvck5XbGpjaXRRTTJnMFdtOUxTekZTZGpRME9WWjBkbGREU25wSVlrMXBWemhKTldJM09VbEZVMHR5UVVsM1NrbFJUR2MxVms4S1dFZGFXbTVFZEc5SlkzVmhZVkI0ZFRCdFFVRjFURmxHYzJsaGRHRmxVMnB5ZW5Sc1dYUlFURll4V2s5V1lqSjNTWEIyTjFoQmNXc0tMUzB0TFMxRlRrUWdRMFZTVkVsR1NVTkJWRVV0TFMwdExRbz0ifX19fQ==",
          "integratedTime": 1668474364,
          "logIndex": 7093563,
          "logID": "c0d23d6ad406973f9559f3ba2d1ca01f84147d8ffc5b8445c224f98b9591801d"
        }
      },
      "Issuer": "https://token.actions.githubusercontent.com",
      "Subject": "https://github.com/chainguard-images/hello-world/.github/workflows/release.yaml@refs/heads/main",
      "githubWorkflowName": "Create Release",
      "githubWorkflowRef": "refs/heads/main",
      "githubWorkflowRepository": "chainguard-images/hello-world",
      "githubWorkflowSha": "6bec98f9e6461695fea1cbba7f1902e148aa221b",
      "githubWorkflowTrigger": "schedule",
      "run_attempt": "1",
      "run_id": "3466520952",
      "sha": "6bec98f9e6461695fea1cbba7f1902e148aa221b"
    }
  }
]
```

You can verify that the image was built in Github Actions in this repository from the `Issuer` and `Subject` fields.
</details>

## Build

This image is built with [melange](https://github.com/chainguard-dev/melange) and [apko](https://github.com/chainguard-dev/apko).

