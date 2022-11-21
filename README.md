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
| `latest` | `sha256:7662148f170dbcc9a957da32c014b97700d53847340773e39c889e60d666aea6`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:7662148f170dbcc9a957da32c014b97700d53847340773e39c889e60d666aea6) | `amd64` `arm64` `armv7` |



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
        "docker-manifest-digest": "sha256:7662148f170dbcc9a957da32c014b97700d53847340773e39c889e60d666aea6"
      },
      "type": "cosign container image signature"
    },
    "optional": {
      "1.3.6.1.4.1.57264.1.1": "https://token.actions.githubusercontent.com",
      "1.3.6.1.4.1.57264.1.2": "schedule",
      "1.3.6.1.4.1.57264.1.3": "07df5554e6134e46a39b7223225de4434f1363ce",
      "1.3.6.1.4.1.57264.1.4": "Create Release",
      "1.3.6.1.4.1.57264.1.5": "chainguard-images/hello-world",
      "1.3.6.1.4.1.57264.1.6": "refs/heads/main",
      "Bundle": {
        "SignedEntryTimestamp": "MEYCIQDzKseZCInxb5zxJolzzIZQ2HlgGcx1P79HhVUFOvlcLQIhANi95/zBtUsyQ5/Y6L/44sQ7RJSZrOmD05fPF4ezoRJh",
        "Payload": {
          "body": "eyJhcGlWZXJzaW9uIjoiMC4wLjEiLCJraW5kIjoiaGFzaGVkcmVrb3JkIiwic3BlYyI6eyJkYXRhIjp7Imhhc2giOnsiYWxnb3JpdGhtIjoic2hhMjU2IiwidmFsdWUiOiIyYWQ4NTgzMDAxZWZiNmIxMTY4ZmQ1OWUzYTBmM2ZkYTgzMmFlYzc0MGUzMGZmYTFjOGQyMGIxNWQyMGE1Y2FmIn19LCJzaWduYXR1cmUiOnsiY29udGVudCI6Ik1FVUNJUUNsbHVOSjZDdkpCRWVBRk0vRHJCcEVmUDFLZ1RoMCtlK1Yyb2oybUNQYytnSWdHVmNoT2VYeXZvMFpmcjhFVzhVM3NDdU1hRXloYVdwMENmRUJ0a254Z3R3PSIsInB1YmxpY0tleSI6eyJjb250ZW50IjoiTFMwdExTMUNSVWRKVGlCRFJWSlVTVVpKUTBGVVJTMHRMUzB0Q2sxSlNVUjBha05EUVhwMVowRjNTVUpCWjBsVlZWWjNWbTV3TnpaTlpVNW9XQzlVWm01Uk9IcHdVMDV4ZEV0VmQwTm5XVWxMYjFwSmVtb3dSVUYzVFhjS1RucEZWazFDVFVkQk1WVkZRMmhOVFdNeWJHNWpNMUoyWTIxVmRWcEhWakpOVWpSM1NFRlpSRlpSVVVSRmVGWjZZVmRrZW1SSE9YbGFVekZ3WW01U2JBcGpiVEZzV2tkc2FHUkhWWGRJYUdOT1RXcEplRTFVU1hoTlJFVjNUbnBCZWxkb1kwNU5ha2w0VFZSSmVFMUVSWGhPZWtGNlYycEJRVTFHYTNkRmQxbElDa3R2V2tsNmFqQkRRVkZaU1V0dldrbDZhakJFUVZGalJGRm5RVVZsUkRGbEt6aFZXbE15YTNKWFVGTlhSemcyVjNWSmMxQnlNbXhCTlRWeVoxbHpiRGtLYzJ4RlpETkVOVlp4WlhKNVdVSmlRMmxDYzI1WFZqUllMM1ZUZVd4dGNXZDBkMVpMY0N0dmFXODBZbVEwTUdWNVdVdFBRMEZzYjNkblowcFhUVUUwUndwQk1WVmtSSGRGUWk5M1VVVkJkMGxJWjBSQlZFSm5UbFpJVTFWRlJFUkJTMEpuWjNKQ1owVkdRbEZqUkVGNlFXUkNaMDVXU0ZFMFJVWm5VVlZoWnpoaUNqRTNWWGxSY1dRelp5OHZNQzltWW5aTU0yaDZjRXROZDBoM1dVUldVakJxUWtKbmQwWnZRVlV6T1ZCd2VqRlphMFZhWWpWeFRtcHdTMFpYYVhocE5Ga0tXa1E0ZDJKUldVUldVakJTUVZGSUwwSkhUWGRaV1ZwbVlVaFNNR05JVFRaTWVUbHVZVmhTYjJSWFNYVlpNamwwVERKT2IxbFhiSFZhTTFab1kyMVJkQXBoVnpGb1dqSldla3d5YUd4aVIzaDJURmhrZG1OdGVHdE1lVFZ1WVZoU2IyUlhTWFprTWpsNVlUSmFjMkl6WkhwTU0wcHNZa2RXYUdNeVZYVmxWMFowQ21KRlFubGFWMXA2VERKb2JGbFhVbnBNTWpGb1lWYzBkMDlSV1V0TGQxbENRa0ZIUkhaNlFVSkJVVkZ5WVVoU01HTklUVFpNZVRrd1lqSjBiR0pwTldnS1dUTlNjR0l5TlhwTWJXUndaRWRvTVZsdVZucGFXRXBxWWpJMU1GcFhOVEJNYlU1MllsUkJWMEpuYjNKQ1owVkZRVmxQTDAxQlJVTkNRV2g2V1RKb2JBcGFTRlp6V2xSQk1rSm5iM0pDWjBWRlFWbFBMMDFCUlVSQ1EyZDNUakpTYlU1VVZURk9SMVV5VFZSTk1GcFVVVEpaVkUwMVdXcGplVTFxVFhsTmFsWnJDbHBVVVRCTmVsSnRUVlJOTWsweVRteE5RbmRIUTJselIwRlJVVUpuTnpoM1FWRlJSVVJyVG5sYVYwWXdXbE5DVTFwWGVHeFpXRTVzVFVOelIwTnBjMGNLUVZGUlFtYzNPSGRCVVZWRlNGZE9iMWxYYkhWYU0xWm9ZMjFSZEdGWE1XaGFNbFo2VERKb2JHSkhlSFpNV0dSMlkyMTRhMDFDTUVkRGFYTkhRVkZSUWdwbk56aDNRVkZaUlVRelNteGFiazEyWVVkV2FGcElUWFppVjBad1ltcERRbWxuV1V0TGQxbENRa0ZJVjJWUlNVVkJaMUk0UWtodlFXVkJRakpCVGpBNUNrMUhja2Q0ZUVWNVdYaHJaVWhLYkc1T2QwdHBVMncyTkROcWVYUXZOR1ZMWTI5QmRrdGxOazlCUVVGQ2FFcGxOV05xTkVGQlFWRkVRVVZqZDFKUlNXZ0tRVTg1YVdSYVUweFRVRlk0WXk5VlJrd3pZUzlyUzJkbGFWZzNNVXN6YlV4bGEyVTBabUppVFZodFZFcEJhVUV3VURrNFMxTk9TREJGZW5BME1UbDROUXBoU25wNldHbHlSbUl3ZGxoMVFrZzJXblU0YlhwSmNtcFBha0ZMUW1kbmNXaHJhazlRVVZGRVFYZE9jRUZFUW0xQmFrVkJNRzU2UTA1clVHeFhTVWt3Q20wNE0zcG5ZMHBNVGxscU9XTTVNek42ZVZWb1JWbFVhRzQxV1ZSR2VXRXlSV3RvYzJscWFHWnZlbGRaU0hGaVJWTnZOVkJCYWtWQmFqVXhVMW93TDBVS1JVZEhaMDFuU21saVpXNXRTRlJ1U1hCclVsUnZhVFJLVjFFMFJYQnBXamxZT1ZCVFZVZzBTR2hSZUdSWmFGRkxNeXR5TkRGd1YxQUtMUzB0TFMxRlRrUWdRMFZTVkVsR1NVTkJWRVV0TFMwdExRbz0ifX19fQ==",
          "integratedTime": 1668992831,
          "logIndex": 7507722,
          "logID": "c0d23d6ad406973f9559f3ba2d1ca01f84147d8ffc5b8445c224f98b9591801d"
        }
      },
      "Issuer": "https://token.actions.githubusercontent.com",
      "Subject": "https://github.com/chainguard-images/hello-world/.github/workflows/release.yaml@refs/heads/main",
      "githubWorkflowName": "Create Release",
      "githubWorkflowRef": "refs/heads/main",
      "githubWorkflowRepository": "chainguard-images/hello-world",
      "githubWorkflowSha": "07df5554e6134e46a39b7223225de4434f1363ce",
      "githubWorkflowTrigger": "schedule",
      "run_attempt": "1",
      "run_id": "3510597327",
      "sha": "07df5554e6134e46a39b7223225de4434f1363ce"
    }
  }
]
```

You can verify that the image was built in Github Actions in this repository from the `Issuer` and `Subject` fields.
</details>

## Build

This image is built with [melange](https://github.com/chainguard-dev/melange) and [apko](https://github.com/chainguard-dev/apko).

