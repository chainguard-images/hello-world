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
| `latest` | `sha256:50740b831ffe5ab7a214489c0b7fe63db6021e1ce7af2c1dc296db716c423222`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:50740b831ffe5ab7a214489c0b7fe63db6021e1ce7af2c1dc296db716c423222) | `amd64` `arm64` `armv7` |



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
        "docker-manifest-digest": "sha256:50740b831ffe5ab7a214489c0b7fe63db6021e1ce7af2c1dc296db716c423222"
      },
      "type": "cosign container image signature"
    },
    "optional": {
      "1.3.6.1.4.1.57264.1.1": "https://token.actions.githubusercontent.com",
      "1.3.6.1.4.1.57264.1.2": "schedule",
      "1.3.6.1.4.1.57264.1.3": "209ac555d713248c62a0c9a41f36c789ccee194c",
      "1.3.6.1.4.1.57264.1.4": "Create Release",
      "1.3.6.1.4.1.57264.1.5": "chainguard-images/hello-world",
      "1.3.6.1.4.1.57264.1.6": "refs/heads/main",
      "Bundle": {
        "SignedEntryTimestamp": "MEYCIQDw9RDM6iEDauZ4BAxnUIfqv6V1bDNmBHAUUoB1QmlLWgIhALMZNI23G3aFDv10W84Up6mn/ZYTvr/n8qVDhi9rVEah",
        "Payload": {
          "body": "eyJhcGlWZXJzaW9uIjoiMC4wLjEiLCJraW5kIjoiaGFzaGVkcmVrb3JkIiwic3BlYyI6eyJkYXRhIjp7Imhhc2giOnsiYWxnb3JpdGhtIjoic2hhMjU2IiwidmFsdWUiOiIxMDZjMGNjZmU0OWZkNjQ1ZTViZmMwMTFmY2FjMGIzODE2OTVjZjkxYjNmZWJlYTFkZGJlOWIzYThiNGFmZGYxIn19LCJzaWduYXR1cmUiOnsiY29udGVudCI6Ik1FVUNJR29lMDdrd1JmYzVaa0QzMzg1aFdNV0xFaHd2dHYxYk10Sk9GdW4vRjVrWEFpRUFrMTdBS1hTRmpITXFyR1laSTFjTDNmOGxES2VqZVQ2MEtNNlFhUUZBOW9FPSIsInB1YmxpY0tleSI6eyJjb250ZW50IjoiTFMwdExTMUNSVWRKVGlCRFJWSlVTVVpKUTBGVVJTMHRMUzB0Q2sxSlNVUjBSRU5EUVhwMVowRjNTVUpCWjBsVlVWZHdSMVJTZWxsNlJtSlJOMHhRWVRJdmVIaHRVVUoyVjFKUmQwTm5XVWxMYjFwSmVtb3dSVUYzVFhjS1RucEZWazFDVFVkQk1WVkZRMmhOVFdNeWJHNWpNMUoyWTIxVmRWcEhWakpOVWpSM1NFRlpSRlpSVVVSRmVGWjZZVmRrZW1SSE9YbGFVekZ3WW01U2JBcGpiVEZzV2tkc2FHUkhWWGRJYUdOT1RXcEplRTFxUVRGTlJFRjRUVlJOZWxkb1kwNU5ha2w0VFdwQk1VMUVRWGxOVkUxNlYycEJRVTFHYTNkRmQxbElDa3R2V2tsNmFqQkRRVkZaU1V0dldrbDZhakJFUVZGalJGRm5RVVZvUjNKaldFbzNSR0o1S3pacmJYRkRXaTgwY0hWNFlraDBXRk5SZFdKSEszZzFkbTRLYldKalJFTkVSeTk2Y1dSdFVYZFRRMHhsTUVoRk5EQm5OMFoxT1RVeFJGaHJOaTlRUzJ4Q1J6QlpPV0Z2Vm5SNWRtRlBRMEZzYjNkblowcFhUVUUwUndwQk1WVmtSSGRGUWk5M1VVVkJkMGxJWjBSQlZFSm5UbFpJVTFWRlJFUkJTMEpuWjNKQ1owVkdRbEZqUkVGNlFXUkNaMDVXU0ZFMFJVWm5VVlZ2SzBoSUNtMW5kV1JoZFZaTFoycFZRVVV3WXpWamFXOUdWRVJ6ZDBoM1dVUldVakJxUWtKbmQwWnZRVlV6T1ZCd2VqRlphMFZhWWpWeFRtcHdTMFpYYVhocE5Ga0tXa1E0ZDJKUldVUldVakJTUVZGSUwwSkhUWGRaV1ZwbVlVaFNNR05JVFRaTWVUbHVZVmhTYjJSWFNYVlpNamwwVERKT2IxbFhiSFZhTTFab1kyMVJkQXBoVnpGb1dqSldla3d5YUd4aVIzaDJURmhrZG1OdGVHdE1lVFZ1WVZoU2IyUlhTWFprTWpsNVlUSmFjMkl6WkhwTU0wcHNZa2RXYUdNeVZYVmxWMFowQ21KRlFubGFWMXA2VERKb2JGbFhVbnBNTWpGb1lWYzBkMDlSV1V0TGQxbENRa0ZIUkhaNlFVSkJVVkZ5WVVoU01HTklUVFpNZVRrd1lqSjBiR0pwTldnS1dUTlNjR0l5TlhwTWJXUndaRWRvTVZsdVZucGFXRXBxWWpJMU1GcFhOVEJNYlU1MllsUkJWMEpuYjNKQ1owVkZRVmxQTDAxQlJVTkNRV2g2V1RKb2JBcGFTRlp6V2xSQk1rSm5iM0pDWjBWRlFWbFBMMDFCUlVSQ1EyZDVUVVJzYUZsNlZURk9WMUV6VFZSTmVVNUVhR3BPYWtwb1RVZE5OVmxVVVhoYWFrMHlDbGw2WXpSUFYwNXFXbGRWZUU5VVVtcE5RbmRIUTJselIwRlJVVUpuTnpoM1FWRlJSVVJyVG5sYVYwWXdXbE5DVTFwWGVHeFpXRTVzVFVOelIwTnBjMGNLUVZGUlFtYzNPSGRCVVZWRlNGZE9iMWxYYkhWYU0xWm9ZMjFSZEdGWE1XaGFNbFo2VERKb2JHSkhlSFpNV0dSMlkyMTRhMDFDTUVkRGFYTkhRVkZSUWdwbk56aDNRVkZaUlVRelNteGFiazEyWVVkV2FGcElUWFppVjBad1ltcERRbWxuV1V0TGQxbENRa0ZJVjJWUlNVVkJaMUk0UWtodlFXVkJRakpCVGpBNUNrMUhja2Q0ZUVWNVdYaHJaVWhLYkc1T2QwdHBVMncyTkROcWVYUXZOR1ZMWTI5QmRrdGxOazlCUVVGQ2FFNHJabkZpT0VGQlFWRkVRVVZqZDFKUlNXZ0tRVTlLTVVkVlUwdDFabVpwYzJWeWJFWlFTR1lyU2tKQmNtaFFWRFJSZEVWb05tRmhjekZxTm5SNU5XMUJhVUU1Y1hoT2NWVXZMM00xV1ZSeWMyNU9OZ3B0TlRad1kwVmlaR3htU1ZZdk1YTTJiR3cyYUZKcFZESkNWRUZMUW1kbmNXaHJhazlRVVZGRVFYZE9ia0ZFUW10QmFrSmlOVUpzWW5ONlNWbFVZMk5rQ21od1VtRXJhMGR0VERaeWRra3hXa014VVhCUmFtMTJNVTlTTTJ4T1RrMTNVRWhZV0djMlJuRkVhWFJOYkVOVk0ybzNUVU5OUVZaRWFqWTVWM0JRY2xFS1RuWndVbVVyVVdKV2MxaEtWMjFOY0ZveGNUUnpNRWRSYjJwMlIzQkZlRmxMS3l0aFJGWkpSalZNYzNKSEsxZDZTMGRtVEcxM1BUMEtMUzB0TFMxRlRrUWdRMFZTVkVsR1NVTkJWRVV0TFMwdExRbz0ifX19fQ==",
          "integratedTime": 1670199106,
          "logIndex": 8417476,
          "logID": "c0d23d6ad406973f9559f3ba2d1ca01f84147d8ffc5b8445c224f98b9591801d"
        }
      },
      "Issuer": "https://token.actions.githubusercontent.com",
      "Subject": "https://github.com/chainguard-images/hello-world/.github/workflows/release.yaml@refs/heads/main",
      "githubWorkflowName": "Create Release",
      "githubWorkflowRef": "refs/heads/main",
      "githubWorkflowRepository": "chainguard-images/hello-world",
      "githubWorkflowSha": "209ac555d713248c62a0c9a41f36c789ccee194c",
      "githubWorkflowTrigger": "schedule",
      "run_attempt": "1",
      "run_id": "3615720982",
      "sha": "209ac555d713248c62a0c9a41f36c789ccee194c"
    }
  }
]
```

You can verify that the image was built in Github Actions in this repository from the `Issuer` and `Subject` fields.
</details>

## Build

This image is built with [melange](https://github.com/chainguard-dev/melange) and [apko](https://github.com/chainguard-dev/apko).

