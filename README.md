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
| `latest` | `sha256:f5f7292be6f85e2363b753d2164d002ad523b053abfdfcd5363c57a83dc6c967`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:f5f7292be6f85e2363b753d2164d002ad523b053abfdfcd5363c57a83dc6c967) | `amd64` `arm64` `armv7` |



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
        "docker-manifest-digest": "sha256:f5f7292be6f85e2363b753d2164d002ad523b053abfdfcd5363c57a83dc6c967"
      },
      "type": "cosign container image signature"
    },
    "optional": {
      "1.3.6.1.4.1.57264.1.1": "https://token.actions.githubusercontent.com",
      "1.3.6.1.4.1.57264.1.2": "schedule",
      "1.3.6.1.4.1.57264.1.3": "4aabd9cadee0a5f2248fe2507165248203229255",
      "1.3.6.1.4.1.57264.1.4": "Create Release",
      "1.3.6.1.4.1.57264.1.5": "chainguard-images/hello-world",
      "1.3.6.1.4.1.57264.1.6": "refs/heads/main",
      "Bundle": {
        "SignedEntryTimestamp": "MEQCIGIKMjvpyNaQG669ABrg0FxanN48jJ4Un03vegsUWk/jAiAk3HSyJCWdutKfsVUMoSY7cfoAS05gSE8poRjlyY+SFg==",
        "Payload": {
          "body": "eyJhcGlWZXJzaW9uIjoiMC4wLjEiLCJraW5kIjoiaGFzaGVkcmVrb3JkIiwic3BlYyI6eyJkYXRhIjp7Imhhc2giOnsiYWxnb3JpdGhtIjoic2hhMjU2IiwidmFsdWUiOiIwNzI3OTA2MGNiZWU2OWFlMTY4ODU4ZmYwZjU4NDdhNjk2OGYzNzUzZmZmZTY4YjlmZWM4NDU3MDRmNmU5MGQyIn19LCJzaWduYXR1cmUiOnsiY29udGVudCI6Ik1FWUNJUUQvRVoyNWNBMXcxZzJKVE9zWmtORE5QS0ZWZ0VwYUV2N0Z1Z2lHVUdvdGlRSWhBTi9qY1VBaUIvU04zWjJkb28yaVU0YU1BNGRuelZSTE52ZkQ3THhxa3cyRCIsInB1YmxpY0tleSI6eyJjb250ZW50IjoiTFMwdExTMUNSVWRKVGlCRFJWSlVTVVpKUTBGVVJTMHRMUzB0Q2sxSlNVUjBWRU5EUVhweFowRjNTVUpCWjBsVlkweHhhazVPYW5vNVJ5dFVPVXRLT0VWbFlrZEpNV3hZYkhWRmQwTm5XVWxMYjFwSmVtb3dSVUYzVFhjS1RucEZWazFDVFVkQk1WVkZRMmhOVFdNeWJHNWpNMUoyWTIxVmRWcEhWakpOVWpSM1NFRlpSRlpSVVVSRmVGWjZZVmRrZW1SSE9YbGFVekZ3WW01U2JBcGpiVEZzV2tkc2FHUkhWWGRJYUdOT1RXcEplRTFxUVRCTlJFRjRUVlJCZVZkb1kwNU5ha2w0VFdwQk1FMUVRWGxOVkVGNVYycEJRVTFHYTNkRmQxbElDa3R2V2tsNmFqQkRRVkZaU1V0dldrbDZhakJFUVZGalJGRm5RVVUyZGswNFRuSndTbmxKY25saVUycHFUMmxIZUU1S01XSndhemxEUWpkUFNGVmliMklLTlhodk1tVmhlRTlIWlc4NGNUaERTSGh6YjNBd1V5c3dZVmxQWWs4M1MwRkhaM1k1WjJ0aVpVTmxPVVZWUTNkUU1HRlBRMEZzYTNkblowcFdUVUUwUndwQk1WVmtSSGRGUWk5M1VVVkJkMGxJWjBSQlZFSm5UbFpJVTFWRlJFUkJTMEpuWjNKQ1owVkdRbEZqUkVGNlFXUkNaMDVXU0ZFMFJVWm5VVlZzT0RkTkNubDFNbnBqV1RaMGFXcFNhWE5YV0dsVWVIZHhVbWRSZDBoM1dVUldVakJxUWtKbmQwWnZRVlV6T1ZCd2VqRlphMFZhWWpWeFRtcHdTMFpYYVhocE5Ga0tXa1E0ZDJKUldVUldVakJTUVZGSUwwSkhUWGRaV1ZwbVlVaFNNR05JVFRaTWVUbHVZVmhTYjJSWFNYVlpNamwwVERKT2IxbFhiSFZhTTFab1kyMVJkQXBoVnpGb1dqSldla3d5YUd4aVIzaDJURmhrZG1OdGVHdE1lVFZ1WVZoU2IyUlhTWFprTWpsNVlUSmFjMkl6WkhwTU0wcHNZa2RXYUdNeVZYVmxWMFowQ21KRlFubGFWMXA2VERKb2JGbFhVbnBNTWpGb1lWYzBkMDlSV1V0TGQxbENRa0ZIUkhaNlFVSkJVVkZ5WVVoU01HTklUVFpNZVRrd1lqSjBiR0pwTldnS1dUTlNjR0l5TlhwTWJXUndaRWRvTVZsdVZucGFXRXBxWWpJMU1GcFhOVEJNYlU1MllsUkJWMEpuYjNKQ1owVkZRVmxQTDAxQlJVTkNRV2g2V1RKb2JBcGFTRlp6V2xSQk1rSm5iM0pDWjBWRlFWbFBMMDFCUlVSQ1EyY3dXVmRHYVZwRWJHcFpWMUpzV2xSQ2FFNVhXWGxOYWxFMFdtMVZlVTVVUVROTlZGa3hDazFxVVRSTmFrRjZUV3BKTlUxcVZURk5RbmRIUTJselIwRlJVVUpuTnpoM1FWRlJSVVJyVG5sYVYwWXdXbE5DVTFwWGVHeFpXRTVzVFVOelIwTnBjMGNLUVZGUlFtYzNPSGRCVVZWRlNGZE9iMWxYYkhWYU0xWm9ZMjFSZEdGWE1XaGFNbFo2VERKb2JHSkhlSFpNV0dSMlkyMTRhMDFDTUVkRGFYTkhRVkZSUWdwbk56aDNRVkZaUlVRelNteGFiazEyWVVkV2FGcElUWFppVjBad1ltcERRbWxSV1V0TGQxbENRa0ZJVjJWUlNVVkJaMUkzUWtoclFXUjNRakZCVGpBNUNrMUhja2Q0ZUVWNVdYaHJaVWhLYkc1T2QwdHBVMncyTkROcWVYUXZOR1ZMWTI5QmRrdGxOazlCUVVGQ2FFNXdOREZGU1VGQlFWRkVRVVZaZDFKQlNXY0tVMkp2VVdkeE9HTTFjbk5pUkZST05tRnZaREpKT0VoRE1sSXpZU3N2WlU4eFZYRkhja3RJY25SelkwTkpRV2cxTUU5WVJYQTNWM016TVVaWE5UQTVkUXAyUjI1RlMwTnZNMW94YzIxdVl6UlVTVzU0ZG5vNGQwRk5RVzlIUTBOeFIxTk5ORGxDUVUxRVFUSnJRVTFIV1VOTlVVUjFXWEYzVVdGcVNWVXZaazFVQ2xFNGRUVm1RbVZDVkZWRFRVZEZMMFJzWTJaUmJHRlBTSEJvZHpSbk9FdDVPV0pKVFVJek5rSm5PWEJhUkVvek4yNTFWVU5OVVVSS2RUTkZaVE5tTkdFS05TOWplVU0yU3l0dlVrTTNTM05wTVVsSmVEZFZPVWxLUWxZeFJGQm9Sekk0ZEVoNk9YaFdaMXAyUWtoaVduWkhhMmxrY21aT1JUMEtMUzB0TFMxRlRrUWdRMFZTVkVsR1NVTkJWRVV0TFMwdExRbz0ifX19fQ==",
          "integratedTime": 1670112671,
          "logIndex": 8384988,
          "logID": "c0d23d6ad406973f9559f3ba2d1ca01f84147d8ffc5b8445c224f98b9591801d"
        }
      },
      "Issuer": "https://token.actions.githubusercontent.com",
      "Subject": "https://github.com/chainguard-images/hello-world/.github/workflows/release.yaml@refs/heads/main",
      "githubWorkflowName": "Create Release",
      "githubWorkflowRef": "refs/heads/main",
      "githubWorkflowRepository": "chainguard-images/hello-world",
      "githubWorkflowSha": "4aabd9cadee0a5f2248fe2507165248203229255",
      "githubWorkflowTrigger": "schedule",
      "run_attempt": "1",
      "run_id": "3610822390",
      "sha": "4aabd9cadee0a5f2248fe2507165248203229255"
    }
  }
]
```

You can verify that the image was built in Github Actions in this repository from the `Issuer` and `Subject` fields.
</details>

## Build

This image is built with [melange](https://github.com/chainguard-dev/melange) and [apko](https://github.com/chainguard-dev/apko).

