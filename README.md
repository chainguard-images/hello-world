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
| `latest` | `sha256:a87e15f62ef95fb9d67bbc1a7ef16710c464640edfad2d38475fdff6f6934800`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:a87e15f62ef95fb9d67bbc1a7ef16710c464640edfad2d38475fdff6f6934800) | `amd64` `arm64` `armv7` |



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
        "docker-manifest-digest": "sha256:a87e15f62ef95fb9d67bbc1a7ef16710c464640edfad2d38475fdff6f6934800"
      },
      "type": "cosign container image signature"
    },
    "optional": {
      "1.3.6.1.4.1.57264.1.1": "https://token.actions.githubusercontent.com",
      "1.3.6.1.4.1.57264.1.2": "schedule",
      "1.3.6.1.4.1.57264.1.3": "9754b4c6910220c0c1a1a2083492369f2dcc155d",
      "1.3.6.1.4.1.57264.1.4": "Create Release",
      "1.3.6.1.4.1.57264.1.5": "chainguard-images/hello-world",
      "1.3.6.1.4.1.57264.1.6": "refs/heads/main",
      "Bundle": {
        "SignedEntryTimestamp": "MEUCIE/IhGqReOIpoNVonsJ/oAGlebNrbBldAYSf5jW7afdyAiEAk/+6M1tAiLpI/ZWDx+NjdpfQ5CnxbUnUu9rfVgeXVNQ=",
        "Payload": {
          "body": "eyJhcGlWZXJzaW9uIjoiMC4wLjEiLCJraW5kIjoiaGFzaGVkcmVrb3JkIiwic3BlYyI6eyJkYXRhIjp7Imhhc2giOnsiYWxnb3JpdGhtIjoic2hhMjU2IiwidmFsdWUiOiJlOTMzMDdjOWVkYWVmYjM2MjA3MWI4NjQ0YTA1NGZjZmE1ZWM2Njg4ZGI5YTNkN2RlOTk5NGU0OGM5YTE4Y2YxIn19LCJzaWduYXR1cmUiOnsiY29udGVudCI6Ik1FUUNJRkNOZlVQMEtZbWFNTWp5SndRSG84L3NmSFlUSWNIQ01mRVVvUVp0M0x1SkFpQnRvaEF1d3pDN1pYT2VTSG54cWM0Tk5sVUE2YkQ0eEpFQ1FKaVphU0hiRmc9PSIsInB1YmxpY0tleSI6eyJjb250ZW50IjoiTFMwdExTMUNSVWRKVGlCRFJWSlVTVVpKUTBGVVJTMHRMUzB0Q2sxSlNVUjBla05EUVhwNVowRjNTVUpCWjBsVlZUUnVRa3A0YUV3MFUySlpaakZhVW10Q2VrSlRUVmxJV1ZkemQwTm5XVWxMYjFwSmVtb3dSVUYzVFhjS1RucEZWazFDVFVkQk1WVkZRMmhOVFdNeWJHNWpNMUoyWTIxVmRWcEhWakpOVWpSM1NFRlpSRlpSVVVSRmVGWjZZVmRrZW1SSE9YbGFVekZ3WW01U2JBcGpiVEZzV2tkc2FHUkhWWGRJYUdOT1RXcEplRTFVVFhkTlJFRjRUWHBGZWxkb1kwNU5ha2w0VFZSTmQwMUVRWGxOZWtWNlYycEJRVTFHYTNkRmQxbElDa3R2V2tsNmFqQkRRVkZaU1V0dldrbDZhakJFUVZGalJGRm5RVVZRUmpjemFtbHpiV0U0YXpWSVNYZ3pWbUZpZDBVelIwOVhiRGh4TUVWRFZVSlRibG9LWnpaeGNIcFJOMUEzVEhCT1FuSkNORlJWUVZCVVZUUXhXRk4wVEdkTFVUVnlka0pTVEZCSlFUQnhZVTlrUzNNMVZqWlBRMEZzYzNkblowcFlUVUUwUndwQk1WVmtSSGRGUWk5M1VVVkJkMGxJWjBSQlZFSm5UbFpJVTFWRlJFUkJTMEpuWjNKQ1owVkdRbEZqUkVGNlFXUkNaMDVXU0ZFMFJVWm5VVlUwYUZsMENrOW9NREpuY2pCclJUQnRRblJVVkV0SlMzWjNNa1JKZDBoM1dVUldVakJxUWtKbmQwWnZRVlV6T1ZCd2VqRlphMFZhWWpWeFRtcHdTMFpYYVhocE5Ga0tXa1E0ZDJKUldVUldVakJTUVZGSUwwSkhUWGRaV1ZwbVlVaFNNR05JVFRaTWVUbHVZVmhTYjJSWFNYVlpNamwwVERKT2IxbFhiSFZhTTFab1kyMVJkQXBoVnpGb1dqSldla3d5YUd4aVIzaDJURmhrZG1OdGVHdE1lVFZ1WVZoU2IyUlhTWFprTWpsNVlUSmFjMkl6WkhwTU0wcHNZa2RXYUdNeVZYVmxWMFowQ21KRlFubGFWMXA2VERKb2JGbFhVbnBNTWpGb1lWYzBkMDlSV1V0TGQxbENRa0ZIUkhaNlFVSkJVVkZ5WVVoU01HTklUVFpNZVRrd1lqSjBiR0pwTldnS1dUTlNjR0l5TlhwTWJXUndaRWRvTVZsdVZucGFXRXBxWWpJMU1GcFhOVEJNYlU1MllsUkJWMEpuYjNKQ1owVkZRVmxQTDAxQlJVTkNRV2g2V1RKb2JBcGFTRlp6V2xSQk1rSm5iM0pDWjBWRlFWbFBMMDFCUlVSQ1EyYzFUbnBWTUZscVVtcE9hbXQ0VFVSSmVVMUhUWGRaZWtab1RWZEZlVTFFWjNwT1JHdDVDazE2V1RWYWFrcHJXVEpOZUU1VVZtdE5RbmRIUTJselIwRlJVVUpuTnpoM1FWRlJSVVJyVG5sYVYwWXdXbE5DVTFwWGVHeFpXRTVzVFVOelIwTnBjMGNLUVZGUlFtYzNPSGRCVVZWRlNGZE9iMWxYYkhWYU0xWm9ZMjFSZEdGWE1XaGFNbFo2VERKb2JHSkhlSFpNV0dSMlkyMTRhMDFDTUVkRGFYTkhRVkZSUWdwbk56aDNRVkZaUlVRelNteGFiazEyWVVkV2FGcElUWFppVjBad1ltcERRbWwzV1V0TGQxbENRa0ZJVjJWUlNVVkJaMUk1UWtoelFXVlJRak5CVGpBNUNrMUhja2Q0ZUVWNVdYaHJaVWhLYkc1T2QwdHBVMncyTkROcWVYUXZOR1ZMWTI5QmRrdGxOazlCUVVGQ2FFMVlhRnBFUVVGQlFWRkVRVVZuZDFKblNXZ0tRVTVCUlc5MFIxWktOVXd2YjJJdmExUkJPVVp0ZGpGVFozQXplSHBIWTFaU2RDOXViUzlQTTBFMVdtWkJhVVZCYmpZMllYcHJSMnhHVURKd1NuTmpNZ3BHUldwdVJHcEVhRWRIZFVJeFIxUTBiazlZY1hGQlZubzNMemgzUTJkWlNVdHZXa2w2YWpCRlFYZE5SR0ZSUVhkYVowbDRRVW92WkhocVdHVmphbWN6Q25ka1lVTmlMMFZJYmpCRE5VOXFPSEJZVDNkT1ZVdE9RbHBDYUcxUVFVNVliRmsxVTJaMFRXTmphMlIxUTFSbE9HVjBOVWxUUVVsNFFVd3ZaR0YyUjNnS2EydGFkMVJQY0M5UGVGcHNkR1JOUVdwaWFtVm9XREZFVG5rMFZuZzFTa042T0RGNWVIUndNMlpVZFVwUWR6VTVZa28xVTJJeVNDczNkejA5Q2kwdExTMHRSVTVFSUVORlVsUkpSa2xEUVZSRkxTMHRMUzBLIn19fX0=",
          "integratedTime": 1669767201,
          "logIndex": 8122057,
          "logID": "c0d23d6ad406973f9559f3ba2d1ca01f84147d8ffc5b8445c224f98b9591801d"
        }
      },
      "Issuer": "https://token.actions.githubusercontent.com",
      "Subject": "https://github.com/chainguard-images/hello-world/.github/workflows/release.yaml@refs/heads/main",
      "githubWorkflowName": "Create Release",
      "githubWorkflowRef": "refs/heads/main",
      "githubWorkflowRepository": "chainguard-images/hello-world",
      "githubWorkflowSha": "9754b4c6910220c0c1a1a2083492369f2dcc155d",
      "githubWorkflowTrigger": "schedule",
      "run_attempt": "1",
      "run_id": "3579084201",
      "sha": "9754b4c6910220c0c1a1a2083492369f2dcc155d"
    }
  }
]
```

You can verify that the image was built in Github Actions in this repository from the `Issuer` and `Subject` fields.
</details>

## Build

This image is built with [melange](https://github.com/chainguard-dev/melange) and [apko](https://github.com/chainguard-dev/apko).

