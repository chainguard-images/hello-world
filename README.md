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
| `latest` | `sha256:bcd525894a5723ce096e67ad3ecec52cf38e5f1405e14c471416a4a98328b583`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:bcd525894a5723ce096e67ad3ecec52cf38e5f1405e14c471416a4a98328b583) | `amd64` `arm64` `armv7` |



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
        "docker-manifest-digest": "sha256:bcd525894a5723ce096e67ad3ecec52cf38e5f1405e14c471416a4a98328b583"
      },
      "type": "cosign container image signature"
    },
    "optional": {
      "1.3.6.1.4.1.57264.1.1": "https://token.actions.githubusercontent.com",
      "1.3.6.1.4.1.57264.1.2": "schedule",
      "1.3.6.1.4.1.57264.1.3": "2dbbb1d71909f70869318039a5d7dac83b3a609f",
      "1.3.6.1.4.1.57264.1.4": "Create Release",
      "1.3.6.1.4.1.57264.1.5": "chainguard-images/hello-world",
      "1.3.6.1.4.1.57264.1.6": "refs/heads/main",
      "Bundle": {
        "SignedEntryTimestamp": "MEUCIQDWvmcnOvGRjodcLeVXSz17bSz4jFLT9Bd7pOFVzENS3QIgPjil2/inf8nJDrurJucCmciyHDO9Lls4UzFe5oCchxs=",
        "Payload": {
          "body": "eyJhcGlWZXJzaW9uIjoiMC4wLjEiLCJraW5kIjoiaGFzaGVkcmVrb3JkIiwic3BlYyI6eyJkYXRhIjp7Imhhc2giOnsiYWxnb3JpdGhtIjoic2hhMjU2IiwidmFsdWUiOiI2ZjdiYWE2ZDI5MDU4ZTg3NjExMTQ5NGRhNzcxNjNjMDg3ZDhiZWFiNWNhMzlhNjVjYzFlY2RjOTE0M2MzYzhmIn19LCJzaWduYXR1cmUiOnsiY29udGVudCI6Ik1FUUNJRUFFOVBpZW5CTVdGM0dqL2Y0K2d2amlVdFVxL3pzeGZUV21lQm05R2c4eEFpQjRqUXBzM0R1THYrcjBBcy9BeEpoZGZQQ3Z0Um02SnVtUjN5a0lXb0w0eHc9PSIsInB1YmxpY0tleSI6eyJjb250ZW50IjoiTFMwdExTMUNSVWRKVGlCRFJWSlVTVVpKUTBGVVJTMHRMUzB0Q2sxSlNVUjBha05EUVhwMVowRjNTVUpCWjBsVldWaHJPV2gzZVVGRlJ6Sk1NMVpTVjBKelIycHRkREpFZERSM2QwTm5XVWxMYjFwSmVtb3dSVUYzVFhjS1RucEZWazFDVFVkQk1WVkZRMmhOVFdNeWJHNWpNMUoyWTIxVmRWcEhWakpOVWpSM1NFRlpSRlpSVVVSRmVGWjZZVmRrZW1SSE9YbGFVekZ3WW01U2JBcGpiVEZzV2tkc2FHUkhWWGRJYUdOT1RXcEplRTFVU1hkTlJFVjNUMVJCTWxkb1kwNU5ha2w0VFZSSmQwMUVSWGhQVkVFeVYycEJRVTFHYTNkRmQxbElDa3R2V2tsNmFqQkRRVkZaU1V0dldrbDZhakJFUVZGalJGRm5RVVZqY0RGcE5VOWlTVmx5Y25Sd2RHbEpZMG92SzBOQmMxRjVhazlNZDFoVlUxRlZaVGdLUWl0eU9DdEhiV2QxWXpscWNFeEpWVE5zVDBKRlZUVktXRTFHYVVWSksxaFBWWFJKZERBM1QzQlFZV3BCZFhwa1ZVdFBRMEZzYjNkblowcFhUVUUwUndwQk1WVmtSSGRGUWk5M1VVVkJkMGxJWjBSQlZFSm5UbFpJVTFWRlJFUkJTMEpuWjNKQ1owVkdRbEZqUkVGNlFXUkNaMDVXU0ZFMFJVWm5VVlUxZVZsdENreGpTR3BZWkdWQ1dIbDZMMU0xYzBScFVHTk1VRGRqZDBoM1dVUldVakJxUWtKbmQwWnZRVlV6T1ZCd2VqRlphMFZhWWpWeFRtcHdTMFpYYVhocE5Ga0tXa1E0ZDJKUldVUldVakJTUVZGSUwwSkhUWGRaV1ZwbVlVaFNNR05JVFRaTWVUbHVZVmhTYjJSWFNYVlpNamwwVERKT2IxbFhiSFZhTTFab1kyMVJkQXBoVnpGb1dqSldla3d5YUd4aVIzaDJURmhrZG1OdGVHdE1lVFZ1WVZoU2IyUlhTWFprTWpsNVlUSmFjMkl6WkhwTU0wcHNZa2RXYUdNeVZYVmxWMFowQ21KRlFubGFWMXA2VERKb2JGbFhVbnBNTWpGb1lWYzBkMDlSV1V0TGQxbENRa0ZIUkhaNlFVSkJVVkZ5WVVoU01HTklUVFpNZVRrd1lqSjBiR0pwTldnS1dUTlNjR0l5TlhwTWJXUndaRWRvTVZsdVZucGFXRXBxWWpJMU1GcFhOVEJNYlU1MllsUkJWMEpuYjNKQ1owVkZRVmxQTDAxQlJVTkNRV2g2V1RKb2JBcGFTRlp6V2xSQk1rSm5iM0pDWjBWRlFWbFBMMDFCUlVSQ1EyZDVXa2RLYVZscVJtdE9la1UxVFVSc2JVNTZRVFJPYW10NlRWUm5kMDE2YkdoT1YxRXpDbHBIUm1wUFJFNXBUVEpGTWsxRWJHMU5RbmRIUTJselIwRlJVVUpuTnpoM1FWRlJSVVJyVG5sYVYwWXdXbE5DVTFwWGVHeFpXRTVzVFVOelIwTnBjMGNLUVZGUlFtYzNPSGRCVVZWRlNGZE9iMWxYYkhWYU0xWm9ZMjFSZEdGWE1XaGFNbFo2VERKb2JHSkhlSFpNV0dSMlkyMTRhMDFDTUVkRGFYTkhRVkZSUWdwbk56aDNRVkZaUlVRelNteGFiazEyWVVkV2FGcElUWFppVjBad1ltcERRbWxuV1V0TGQxbENRa0ZJVjJWUlNVVkJaMUk0UWtodlFXVkJRakpCVGpBNUNrMUhja2Q0ZUVWNVdYaHJaVWhLYkc1T2QwdHBVMncyTkROcWVYUXZOR1ZMWTI5QmRrdGxOazlCUVVGQ2FFcExWVGx4VVVGQlFWRkVRVVZqZDFKUlNXZ0tRVTV1VEZkUmJGSnBVRkJtVEUxeWNDdDNNbkpLTmtrMFJXUXZWSFJ5UVd3d1ZGaFllbTVSVDNaRGNXZEJhVUZ1V1RWSE9EQnFkV1JWUzFSM1pGQnFSd3BVUkdadE5YVmhRMlZKZG5WMVpVbzNNa2MwTUhsNmVtTjRla0ZMUW1kbmNXaHJhazlRVVZGRVFYZE9jRUZFUW0xQmFrVkJiVXRDZDFVd1VFc3JVMUJMQ2s1aVVqbHhjM1V6YzI1VlltTnZZMlJDZUdGTlZHNVFTbkJoTDFkNFNIaGtlbTlpVlRSelJuSjRaeXRXTDAxNVJHVXhVa2RCYWtWQmVHUmhOV1ZZZUhZS1dqVmhSblYxTWxWNlMxWTRlQ3RXZG5CSVlTdGlSMUphV2xkMldVOUdNazFQVkdscFNrRm9UMUpWSzBKT1Rua3ZRM3BYY2xjNVVXY0tMUzB0TFMxRlRrUWdRMFZTVkVsR1NVTkJWRVV0TFMwdExRbz0ifX19fQ==",
          "integratedTime": 1668906556,
          "logIndex": 7449065,
          "logID": "c0d23d6ad406973f9559f3ba2d1ca01f84147d8ffc5b8445c224f98b9591801d"
        }
      },
      "Issuer": "https://token.actions.githubusercontent.com",
      "Subject": "https://github.com/chainguard-images/hello-world/.github/workflows/release.yaml@refs/heads/main",
      "githubWorkflowName": "Create Release",
      "githubWorkflowRef": "refs/heads/main",
      "githubWorkflowRepository": "chainguard-images/hello-world",
      "githubWorkflowSha": "2dbbb1d71909f70869318039a5d7dac83b3a609f",
      "githubWorkflowTrigger": "schedule",
      "run_attempt": "1",
      "run_id": "3505887314",
      "sha": "2dbbb1d71909f70869318039a5d7dac83b3a609f"
    }
  }
]
```

You can verify that the image was built in Github Actions in this repository from the `Issuer` and `Subject` fields.
</details>

## Build

This image is built with [melange](https://github.com/chainguard-dev/melange) and [apko](https://github.com/chainguard-dev/apko).

