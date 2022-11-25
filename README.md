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
| `latest` | `sha256:63c6c1a5c0ad391024c5ac61cfd116c7fcc64a8515bdccbe037cfcb65f4887a6`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:63c6c1a5c0ad391024c5ac61cfd116c7fcc64a8515bdccbe037cfcb65f4887a6) | `amd64` `arm64` `armv7` |



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
        "docker-manifest-digest": "sha256:63c6c1a5c0ad391024c5ac61cfd116c7fcc64a8515bdccbe037cfcb65f4887a6"
      },
      "type": "cosign container image signature"
    },
    "optional": {
      "1.3.6.1.4.1.57264.1.1": "https://token.actions.githubusercontent.com",
      "1.3.6.1.4.1.57264.1.2": "schedule",
      "1.3.6.1.4.1.57264.1.3": "30f4a91a8736b50a3e1113f8f50857d780b4e4ea",
      "1.3.6.1.4.1.57264.1.4": "Create Release",
      "1.3.6.1.4.1.57264.1.5": "chainguard-images/hello-world",
      "1.3.6.1.4.1.57264.1.6": "refs/heads/main",
      "Bundle": {
        "SignedEntryTimestamp": "MEUCIHvfp9h3FrqS1F7QbGT2qGfXIX5MQVE6+PNqvOJS9vjpAiEAqAtDZ8MoHlA9Uj9nT2Wuw8uPNlHY5jd3LRq39SeI/PA=",
        "Payload": {
          "body": "eyJhcGlWZXJzaW9uIjoiMC4wLjEiLCJraW5kIjoiaGFzaGVkcmVrb3JkIiwic3BlYyI6eyJkYXRhIjp7Imhhc2giOnsiYWxnb3JpdGhtIjoic2hhMjU2IiwidmFsdWUiOiJiMmYxOGE0NzgyNzNhZWIyMWUzYWUyNDcwYzJmMThmNWY5ZDQ3OWIyMDE3ZTJkODU3YzFjYmVmYzQzYTkwN2RmIn19LCJzaWduYXR1cmUiOnsiY29udGVudCI6Ik1FWUNJUUNHR05DRDRtSXJhVS9SVlpoT0YrQTJXYzdoK0hEYXA4VGxzTWpWQkVlS3VnSWhBT1lieWgxTVc1cHVvNktQbDVGTzZ0aVFqSTNlWmY2Qko4NFpobllHWXE4ZiIsInB1YmxpY0tleSI6eyJjb250ZW50IjoiTFMwdExTMUNSVWRKVGlCRFJWSlVTVVpKUTBGVVJTMHRMUzB0Q2sxSlNVUjBWRU5EUVhwMVowRjNTVUpCWjBsVlVtcFJaRzlRZUdkdGRGQktTbkIxTkROeVFraFZZVmx4VVZOQmQwTm5XVWxMYjFwSmVtb3dSVUYzVFhjS1RucEZWazFDVFVkQk1WVkZRMmhOVFdNeWJHNWpNMUoyWTIxVmRWcEhWakpOVWpSM1NFRlpSRlpSVVVSRmVGWjZZVmRrZW1SSE9YbGFVekZ3WW01U2JBcGpiVEZzV2tkc2FHUkhWWGRJYUdOT1RXcEplRTFVU1RGTlJFRjRUVlJCTWxkb1kwNU5ha2w0VFZSSk1VMUVRWGxOVkVFeVYycEJRVTFHYTNkRmQxbElDa3R2V2tsNmFqQkRRVkZaU1V0dldrbDZhakJFUVZGalJGRm5RVVZDTVRkemVVOU5SamxzYUVoNGIwRlFZVTlIWkdaNk5qRjRUbXhpYkM5M1ZFVlVVWEVLSzBkUFQwODVaRXB1VHl0cEt6TkJhbkIxVjNsdmFqRjZOSE16Wkc5MmRtNW5WMU5oZG5sMlJ6WjVSMlJOVUV0UFVVdFBRMEZzYjNkblowcFhUVUUwUndwQk1WVmtSSGRGUWk5M1VVVkJkMGxJWjBSQlZFSm5UbFpJVTFWRlJFUkJTMEpuWjNKQ1owVkdRbEZqUkVGNlFXUkNaMDVXU0ZFMFJVWm5VVlZCTUV4NENuUndUR3R1WW5GTmRscFdXRFZEYms1cEwyTmtUR1JWZDBoM1dVUldVakJxUWtKbmQwWnZRVlV6T1ZCd2VqRlphMFZhWWpWeFRtcHdTMFpYYVhocE5Ga0tXa1E0ZDJKUldVUldVakJTUVZGSUwwSkhUWGRaV1ZwbVlVaFNNR05JVFRaTWVUbHVZVmhTYjJSWFNYVlpNamwwVERKT2IxbFhiSFZhTTFab1kyMVJkQXBoVnpGb1dqSldla3d5YUd4aVIzaDJURmhrZG1OdGVHdE1lVFZ1WVZoU2IyUlhTWFprTWpsNVlUSmFjMkl6WkhwTU0wcHNZa2RXYUdNeVZYVmxWMFowQ21KRlFubGFWMXA2VERKb2JGbFhVbnBNTWpGb1lWYzBkMDlSV1V0TGQxbENRa0ZIUkhaNlFVSkJVVkZ5WVVoU01HTklUVFpNZVRrd1lqSjBiR0pwTldnS1dUTlNjR0l5TlhwTWJXUndaRWRvTVZsdVZucGFXRXBxWWpJMU1GcFhOVEJNYlU1MllsUkJWMEpuYjNKQ1owVkZRVmxQTDAxQlJVTkNRV2g2V1RKb2JBcGFTRlp6V2xSQk1rSm5iM0pDWjBWRlFWbFBMMDFCUlVSQ1EyZDZUVWRaTUZsVWEzaFpWR2N6VFhwYWFVNVVRbWhOTWxWNFRWUkZlbHBxYUcxT1ZFRTBDazVVWkd0T2VtZDNXV3BTYkU1SFZtaE5RbmRIUTJselIwRlJVVUpuTnpoM1FWRlJSVVJyVG5sYVYwWXdXbE5DVTFwWGVHeFpXRTVzVFVOelIwTnBjMGNLUVZGUlFtYzNPSGRCVVZWRlNGZE9iMWxYYkhWYU0xWm9ZMjFSZEdGWE1XaGFNbFo2VERKb2JHSkhlSFpNV0dSMlkyMTRhMDFDTUVkRGFYTkhRVkZSUWdwbk56aDNRVkZaUlVRelNteGFiazEyWVVkV2FGcElUWFppVjBad1ltcERRbWxuV1V0TGQxbENRa0ZJVjJWUlNVVkJaMUk0UWtodlFXVkJRakpCVGpBNUNrMUhja2Q0ZUVWNVdYaHJaVWhLYkc1T2QwdHBVMncyTkROcWVYUXZOR1ZMWTI5QmRrdGxOazlCUVVGQ2FFdDNabkI2TkVGQlFWRkVRVVZqZDFKUlNXZ0tRVW96WW01TE1YcFJZWHBySzFKNmVHaFRRMEYwUm1vM00yb3hUR2RwVFZBdlJGZG9TelJEYzAxMU56RkJhVUoxVFZWNlVsWlhOMlo1UmpSQ01FRnZXZ3B3VTBkemVUWmtjalYxTVc5TU1VTkxkVXN5T0RZeVYzcHZWRUZMUW1kbmNXaHJhazlRVVZGRVFYZE9iMEZFUW14QmFrVkJNMlZ3WTNreFdFTTRabWh6Q21OMVJ6ZHRPWHBpTWpRMk9Tc3pOSEpIWXpVd1lWbDFPRXNyYld4UlJHNU1TRzVZTkdKVFZVNUJOVFZEZVRoWFVVUmhOVmRCYWtGa2NtRTRLMHBXUjNBS2VtMVBNRlpPTkdaNVVsazRha0ZyTUhoT1VsZEdWME55YVRoWWJITkVZMGt3Wkdad0t6QlJiakIxV201amNVTTRhM0YyVFhjeE9EMEtMUzB0TFMxRlRrUWdRMFZTVkVsR1NVTkJWRVV0TFMwdExRbz0ifX19fQ==",
          "integratedTime": 1669335074,
          "logIndex": 7791055,
          "logID": "c0d23d6ad406973f9559f3ba2d1ca01f84147d8ffc5b8445c224f98b9591801d"
        }
      },
      "Issuer": "https://token.actions.githubusercontent.com",
      "Subject": "https://github.com/chainguard-images/hello-world/.github/workflows/release.yaml@refs/heads/main",
      "githubWorkflowName": "Create Release",
      "githubWorkflowRef": "refs/heads/main",
      "githubWorkflowRepository": "chainguard-images/hello-world",
      "githubWorkflowSha": "30f4a91a8736b50a3e1113f8f50857d780b4e4ea",
      "githubWorkflowTrigger": "schedule",
      "run_attempt": "1",
      "run_id": "3544333823",
      "sha": "30f4a91a8736b50a3e1113f8f50857d780b4e4ea"
    }
  }
]
```

You can verify that the image was built in Github Actions in this repository from the `Issuer` and `Subject` fields.
</details>

## Build

This image is built with [melange](https://github.com/chainguard-dev/melange) and [apko](https://github.com/chainguard-dev/apko).

