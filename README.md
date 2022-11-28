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
| `latest` | `sha256:ae5a24265c67133010387d1a01c7ed346dd3f6c1b22abe919ca5115f9f29bb91`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:ae5a24265c67133010387d1a01c7ed346dd3f6c1b22abe919ca5115f9f29bb91) | `amd64` `arm64` `armv7` |



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
        "docker-manifest-digest": "sha256:ae5a24265c67133010387d1a01c7ed346dd3f6c1b22abe919ca5115f9f29bb91"
      },
      "type": "cosign container image signature"
    },
    "optional": {
      "1.3.6.1.4.1.57264.1.1": "https://token.actions.githubusercontent.com",
      "1.3.6.1.4.1.57264.1.2": "schedule",
      "1.3.6.1.4.1.57264.1.3": "e72a7a2ab44be9596ca5d7ebdfdee1c4e572e18a",
      "1.3.6.1.4.1.57264.1.4": "Create Release",
      "1.3.6.1.4.1.57264.1.5": "chainguard-images/hello-world",
      "1.3.6.1.4.1.57264.1.6": "refs/heads/main",
      "Bundle": {
        "SignedEntryTimestamp": "MEQCIG1AkSpoE7S1gWVNtkGaTtF0B5fx70+IKvr2UzpOQTg0AiACAoKwsGilvZLJSOMuwvOwXJ2PLmzDhYQw2QBJUpWmyg==",
        "Payload": {
          "body": "eyJhcGlWZXJzaW9uIjoiMC4wLjEiLCJraW5kIjoiaGFzaGVkcmVrb3JkIiwic3BlYyI6eyJkYXRhIjp7Imhhc2giOnsiYWxnb3JpdGhtIjoic2hhMjU2IiwidmFsdWUiOiI0MGE3MGI2NDlkODhhMGM1M2I1OGMyZDY5ZWFhNjI3YjVhMmVkYmJmNGEzMzZmMTY1NDVlMWVkOGU0ODc0NjI3In19LCJzaWduYXR1cmUiOnsiY29udGVudCI6Ik1FVUNJUUM4cndWZDVyOTJ4a2VtNFZPMnlhVWtPY25NdFJZcG9Kdk1Pb2FnaHJXVVFBSWdhclJ5cmtOVVgxT2RieUQ4U3NNN2Zac2hsTnh6NDk2YnpRZEZtM2NtQ1pzPSIsInB1YmxpY0tleSI6eyJjb250ZW50IjoiTFMwdExTMUNSVWRKVGlCRFJWSlVTVVpKUTBGVVJTMHRMUzB0Q2sxSlNVUjBha05EUVhwNVowRjNTVUpCWjBsVldqZFdUek41TmsxRGVtNVNOVk5wTVd0M1dGcE9jM1UxSzB0M2QwTm5XVWxMYjFwSmVtb3dSVUYzVFhjS1RucEZWazFDVFVkQk1WVkZRMmhOVFdNeWJHNWpNMUoyWTIxVmRWcEhWakpOVWpSM1NFRlpSRlpSVVVSRmVGWjZZVmRrZW1SSE9YbGFVekZ3WW01U2JBcGpiVEZzV2tkc2FHUkhWWGRJYUdOT1RXcEplRTFVU1RSTlJFRjRUVlJWTTFkb1kwNU5ha2w0VFZSSk5FMUVRWGxOVkZVelYycEJRVTFHYTNkRmQxbElDa3R2V2tsNmFqQkRRVkZaU1V0dldrbDZhakJFUVZGalJGRm5RVVZvU2xCV2IzbENTazFFV1dkNFEyaGFNa3hwT0RkM2REWnNNRTVFVDBSQ2EybDJXR2NLVlRRNGJESmlhVTR5WVVoNE9FaE5UMHRZZGtSdldYaDNVREIwY2s1MldFTnRaRTlDVEU5b0wzcFdVa3ROVldoQmFuRlBRMEZzYzNkblowcFlUVUUwUndwQk1WVmtSSGRGUWk5M1VVVkJkMGxJWjBSQlZFSm5UbFpJVTFWRlJFUkJTMEpuWjNKQ1owVkdRbEZqUkVGNlFXUkNaMDVXU0ZFMFJVWm5VVlZGUWtoRENubEtTVXBrZFRSWE1td3pSWE5uZGtWUWFXZDNMM0p2ZDBoM1dVUldVakJxUWtKbmQwWnZRVlV6T1ZCd2VqRlphMFZhWWpWeFRtcHdTMFpYYVhocE5Ga0tXa1E0ZDJKUldVUldVakJTUVZGSUwwSkhUWGRaV1ZwbVlVaFNNR05JVFRaTWVUbHVZVmhTYjJSWFNYVlpNamwwVERKT2IxbFhiSFZhTTFab1kyMVJkQXBoVnpGb1dqSldla3d5YUd4aVIzaDJURmhrZG1OdGVHdE1lVFZ1WVZoU2IyUlhTWFprTWpsNVlUSmFjMkl6WkhwTU0wcHNZa2RXYUdNeVZYVmxWMFowQ21KRlFubGFWMXA2VERKb2JGbFhVbnBNTWpGb1lWYzBkMDlSV1V0TGQxbENRa0ZIUkhaNlFVSkJVVkZ5WVVoU01HTklUVFpNZVRrd1lqSjBiR0pwTldnS1dUTlNjR0l5TlhwTWJXUndaRWRvTVZsdVZucGFXRXBxWWpJMU1GcFhOVEJNYlU1MllsUkJWMEpuYjNKQ1owVkZRVmxQTDAxQlJVTkNRV2g2V1RKb2JBcGFTRlp6V2xSQk1rSm5iM0pDWjBWRlFWbFBMMDFCUlVSQ1EyaHNUbnBLYUU0eVJYbFpWMGt3VGtkS2JFOVVWVFZPYlU1b1RsZFJNMXBYU210YWJWSnNDbHBVUm1wT1IxVXhUbnBLYkUxVWFHaE5RbmRIUTJselIwRlJVVUpuTnpoM1FWRlJSVVJyVG5sYVYwWXdXbE5DVTFwWGVHeFpXRTVzVFVOelIwTnBjMGNLUVZGUlFtYzNPSGRCVVZWRlNGZE9iMWxYYkhWYU0xWm9ZMjFSZEdGWE1XaGFNbFo2VERKb2JHSkhlSFpNV0dSMlkyMTRhMDFDTUVkRGFYTkhRVkZSUWdwbk56aDNRVkZaUlVRelNteGFiazEyWVVkV2FGcElUWFppVjBad1ltcERRbWwzV1V0TGQxbENRa0ZJVjJWUlNVVkJaMUk1UWtoelFXVlJRak5CVGpBNUNrMUhja2Q0ZUVWNVdYaHJaVWhLYkc1T2QwdHBVMncyTkROcWVYUXZOR1ZMWTI5QmRrdGxOazlCUVVGQ2FFeDFWR2Q0WTBGQlFWRkVRVVZuZDFKblNXZ0tRVkJVUlVzeVluSldWRmx4SzJOV1FUSTNhVEo1VDFCSFJtOXJja3hKYTJST2FVTkZjVWg2WTFBNWJ5dEJhVVZCYWpSd1JVeENabEJFVWpsRE1YVTBaZ3AxYzB0V2EyeEtOVkJZU3pabVUxRm5VRkJFTUhWNFJqTTRjbmQzUTJkWlNVdHZXa2w2YWpCRlFYZE5SR0ZCUVhkYVVVbDNabXhrVXpWSlptUnRZbTB4Q21wWE9XODBXblZJTUV4bmVYWnZhVzR4VEcweFQydFdRU3QzTkhsTFlUVkdXbGh1TkhsQ1dGbFJRbXhXU0VKR1RqazVlRmhCYWtWQmFETTRMM2hUUkhBS1Qwd3habUpWZUdGUFVETlBja0YzTUV4dmRHMUVZVzV0T0ZGd2VWcERORFJhY1VKM2NXeERaMHRNWkN0cWQwRm9jV2Q0T1hsU2NuRUtMUzB0TFMxRlRrUWdRMFZTVkVsR1NVTkJWRVV0TFMwdExRbz0ifX19fQ==",
          "integratedTime": 1669594325,
          "logIndex": 7977237,
          "logID": "c0d23d6ad406973f9559f3ba2d1ca01f84147d8ffc5b8445c224f98b9591801d"
        }
      },
      "Issuer": "https://token.actions.githubusercontent.com",
      "Subject": "https://github.com/chainguard-images/hello-world/.github/workflows/release.yaml@refs/heads/main",
      "githubWorkflowName": "Create Release",
      "githubWorkflowRef": "refs/heads/main",
      "githubWorkflowRepository": "chainguard-images/hello-world",
      "githubWorkflowSha": "e72a7a2ab44be9596ca5d7ebdfdee1c4e572e18a",
      "githubWorkflowTrigger": "schedule",
      "run_attempt": "1",
      "run_id": "3560593149",
      "sha": "e72a7a2ab44be9596ca5d7ebdfdee1c4e572e18a"
    }
  }
]
```

You can verify that the image was built in Github Actions in this repository from the `Issuer` and `Subject` fields.
</details>

## Build

This image is built with [melange](https://github.com/chainguard-dev/melange) and [apko](https://github.com/chainguard-dev/apko).

