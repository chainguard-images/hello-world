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
| `latest` | `sha256:170c160e7ab94f57aa99e12c5c21c4f31b8d48d4b982d72015708947ca2904e1`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:170c160e7ab94f57aa99e12c5c21c4f31b8d48d4b982d72015708947ca2904e1) | `amd64` `arm64` `armv7` |



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
        "docker-manifest-digest": "sha256:170c160e7ab94f57aa99e12c5c21c4f31b8d48d4b982d72015708947ca2904e1"
      },
      "type": "cosign container image signature"
    },
    "optional": {
      "1.3.6.1.4.1.57264.1.1": "https://token.actions.githubusercontent.com",
      "1.3.6.1.4.1.57264.1.2": "schedule",
      "1.3.6.1.4.1.57264.1.3": "2ece71b96d260e850e3153463cbe2e9b14440b4d",
      "1.3.6.1.4.1.57264.1.4": "Create Release",
      "1.3.6.1.4.1.57264.1.5": "chainguard-images/hello-world",
      "1.3.6.1.4.1.57264.1.6": "refs/heads/main",
      "Bundle": {
        "SignedEntryTimestamp": "MEYCIQD7ftdBlG/KNHutp9bChTXORvmbH1R6A4ECSU1gqVukLgIhALJt+LsVcKTfnGQl24pGKo8D61mpb5A9H3al1Qy93iA7",
        "Payload": {
          "body": "eyJhcGlWZXJzaW9uIjoiMC4wLjEiLCJraW5kIjoiaGFzaGVkcmVrb3JkIiwic3BlYyI6eyJkYXRhIjp7Imhhc2giOnsiYWxnb3JpdGhtIjoic2hhMjU2IiwidmFsdWUiOiIwMzNjNzJjYmFlMzUzNmYyYTFmZDllNWFmNWE0MWZlOTU2NWQ2MGIwYWYyMDRhZTBlMzNkOTA1MDM4ZmE5MjBmIn19LCJzaWduYXR1cmUiOnsiY29udGVudCI6Ik1FVUNJUURqYUVTTWEydkxOM3MvVEU4TnZxaGtzSlA3L1N2bkZPVnBUWTBZRCtPSWxBSWdPeFpxM0JpeTZ5STYzSWI0Qktpb3NsZUJwazBSZzFUYW9zMStlNDJmMEhjPSIsInB1YmxpY0tleSI6eyJjb250ZW50IjoiTFMwdExTMUNSVWRKVGlCRFJWSlVTVVpKUTBGVVJTMHRMUzB0Q2sxSlNVUjBha05EUVhwNVowRjNTVUpCWjBsVlYwazJXQzluUkVwU2FtMU5iRkpaTTFCRGVYazNNbWhuVTFSbmQwTm5XVWxMYjFwSmVtb3dSVUYzVFhjS1RucEZWazFDVFVkQk1WVkZRMmhOVFdNeWJHNWpNMUoyWTIxVmRWcEhWakpOVWpSM1NFRlpSRlpSVVVSRmVGWjZZVmRrZW1SSE9YbGFVekZ3WW01U2JBcGpiVEZzV2tkc2FHUkhWWGRJYUdOT1RXcEplRTFxUVhoTlJFRjRUV3BKZUZkb1kwNU5ha2w0VFdwQmVFMUVRWGxOYWtsNFYycEJRVTFHYTNkRmQxbElDa3R2V2tsNmFqQkRRVkZaU1V0dldrbDZhakJFUVZGalJGRm5RVVZ0THpoc00zWnBPR0pqVlZKT2FVczRPSEJwZEhwbk1uZFRZalV3WkZOWWMyZExNSGNLU21NeUwyMXJaRE5yZGxoSE5UUlpiVlJMWVdWUWNtOW9PRFZTSzJKa1VsTkhaV0l6YUc1dU0zQlpaMmgyVUZoRWQzRlBRMEZzYzNkblowcFlUVUUwUndwQk1WVmtSSGRGUWk5M1VVVkJkMGxJWjBSQlZFSm5UbFpJVTFWRlJFUkJTMEpuWjNKQ1owVkdRbEZqUkVGNlFXUkNaMDVXU0ZFMFJVWm5VVlZKYWsxSUNubE1MMk5RYkdab2JteE9WMUE1UVRGQk0xaGhVbHBKZDBoM1dVUldVakJxUWtKbmQwWnZRVlV6T1ZCd2VqRlphMFZhWWpWeFRtcHdTMFpYYVhocE5Ga0tXa1E0ZDJKUldVUldVakJTUVZGSUwwSkhUWGRaV1ZwbVlVaFNNR05JVFRaTWVUbHVZVmhTYjJSWFNYVlpNamwwVERKT2IxbFhiSFZhTTFab1kyMVJkQXBoVnpGb1dqSldla3d5YUd4aVIzaDJURmhrZG1OdGVHdE1lVFZ1WVZoU2IyUlhTWFprTWpsNVlUSmFjMkl6WkhwTU0wcHNZa2RXYUdNeVZYVmxWMFowQ21KRlFubGFWMXA2VERKb2JGbFhVbnBNTWpGb1lWYzBkMDlSV1V0TGQxbENRa0ZIUkhaNlFVSkJVVkZ5WVVoU01HTklUVFpNZVRrd1lqSjBiR0pwTldnS1dUTlNjR0l5TlhwTWJXUndaRWRvTVZsdVZucGFXRXBxWWpJMU1GcFhOVEJNYlU1MllsUkJWMEpuYjNKQ1owVkZRVmxQTDAxQlJVTkNRV2g2V1RKb2JBcGFTRlp6V2xSQk1rSm5iM0pDWjBWRlFWbFBMMDFCUlVSQ1EyZDVXbGRPYkU1NlJtbFBWRnByVFdwWmQxcFVaekZOUjFWNlRWUlZlazVFV1hwWk1rcHNDazF0VlRWWmFrVXdUa1JSZDFscVVtdE5RbmRIUTJselIwRlJVVUpuTnpoM1FWRlJSVVJyVG5sYVYwWXdXbE5DVTFwWGVHeFpXRTVzVFVOelIwTnBjMGNLUVZGUlFtYzNPSGRCVVZWRlNGZE9iMWxYYkhWYU0xWm9ZMjFSZEdGWE1XaGFNbFo2VERKb2JHSkhlSFpNV0dSMlkyMTRhMDFDTUVkRGFYTkhRVkZSUWdwbk56aDNRVkZaUlVRelNteGFiazEyWVVkV2FGcElUWFppVjBad1ltcERRbWwzV1V0TGQxbENRa0ZJVjJWUlNVVkJaMUk1UWtoelFXVlJRak5CVGpBNUNrMUhja2Q0ZUVWNVdYaHJaVWhLYkc1T2QwdHBVMncyTkROcWVYUXZOR1ZMWTI5QmRrdGxOazlCUVVGQ2FFMXpSemxyV1VGQlFWRkVRVVZuZDFKblNXZ0tRVkJPTlhGT2NVNTFiVTFsZW5GRWNVNXZZVEZHTjJzdmRuUkllV0ZXWkRkbFRHWnNXRVpaUVRKTmVucEJhVVZCTDFCR2FGUm1NekYzVEVndmQza3pTUXA2UVd4SVIySTBOa3RqZVU5WlZ6ZENjMDlUT1VsRGQweDVka0YzUTJkWlNVdHZXa2w2YWpCRlFYZE5SR0ZCUVhkYVVVbDNUakoyY1dJeFdVSjNWVTFXQ25KNlZYTnJjelZsWm10c09GVTJWbEpPU0d4blpGcHpiamN6VWpsM1VYTnJiMGRyZFVKeGJ6RTVjMGxCTmxJM2Vsa3JkUzlCYWtWQk9FWnFRalJMYmxnS05USTNTV1JxZEdvd1UxaHNUMlpzV1c1ek1IVlZSVEpqVDJwd1pDOWhOVGN5WWtoeFNVdExkMVJoY2tSYU0yeDRRa3BRZGxCMlNtc0tMUzB0TFMxRlRrUWdRMFZTVkVsR1NVTkJWRVV0TFMwdExRbz0ifX19fQ==",
          "integratedTime": 1669853552,
          "logIndex": 8188278,
          "logID": "c0d23d6ad406973f9559f3ba2d1ca01f84147d8ffc5b8445c224f98b9591801d"
        }
      },
      "Issuer": "https://token.actions.githubusercontent.com",
      "Subject": "https://github.com/chainguard-images/hello-world/.github/workflows/release.yaml@refs/heads/main",
      "githubWorkflowName": "Create Release",
      "githubWorkflowRef": "refs/heads/main",
      "githubWorkflowRepository": "chainguard-images/hello-world",
      "githubWorkflowSha": "2ece71b96d260e850e3153463cbe2e9b14440b4d",
      "githubWorkflowTrigger": "schedule",
      "run_attempt": "1",
      "run_id": "3588175960",
      "sha": "2ece71b96d260e850e3153463cbe2e9b14440b4d"
    }
  }
]
```

You can verify that the image was built in Github Actions in this repository from the `Issuer` and `Subject` fields.
</details>

## Build

This image is built with [melange](https://github.com/chainguard-dev/melange) and [apko](https://github.com/chainguard-dev/apko).

