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
| `latest` | `sha256:bc5c717039f2e9d61dd3746ee4d23fb63a6fe214e971824945f76ff565a86835`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:bc5c717039f2e9d61dd3746ee4d23fb63a6fe214e971824945f76ff565a86835) | `amd64` `arm64` `armv7` |



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
        "docker-manifest-digest": "sha256:bc5c717039f2e9d61dd3746ee4d23fb63a6fe214e971824945f76ff565a86835"
      },
      "type": "cosign container image signature"
    },
    "optional": {
      "1.3.6.1.4.1.57264.1.1": "https://token.actions.githubusercontent.com",
      "1.3.6.1.4.1.57264.1.2": "schedule",
      "1.3.6.1.4.1.57264.1.3": "e6c7720a226868478d76d0c73462894ea3aca767",
      "1.3.6.1.4.1.57264.1.4": "Create Release",
      "1.3.6.1.4.1.57264.1.5": "chainguard-images/hello-world",
      "1.3.6.1.4.1.57264.1.6": "refs/heads/main",
      "Bundle": {
        "SignedEntryTimestamp": "MEYCIQCkuatG7igQMdXqlYnONvth8vBJJKaSWT5vYYwbkCEdwgIhAI7sdDpPnByDJeoAPlQxpXeqIbyaMWhk2zP5C+CGT4mO",
        "Payload": {
          "body": "eyJhcGlWZXJzaW9uIjoiMC4wLjEiLCJraW5kIjoiaGFzaGVkcmVrb3JkIiwic3BlYyI6eyJkYXRhIjp7Imhhc2giOnsiYWxnb3JpdGhtIjoic2hhMjU2IiwidmFsdWUiOiJhYjI4MDkxZWM1ODY4YzJiNjEyNzc3OTdlYTVjZWMyM2RjZTc4YzRlMTQyOWI3MWYyMzg2ZmNlMzNjN2IwODI2In19LCJzaWduYXR1cmUiOnsiY29udGVudCI6Ik1FVUNJQ1dCVkpIVi9VZW5SckxuMHkzUStWWGFFSHpxcTlCTjZ3em4vaVl6S1RtekFpRUF3NkdIeHc5b2orVExNaS9jK0xGVDNibjBmakVGZTk4U1R1T09xNVJkSnJNPSIsInB1YmxpY0tleSI6eyJjb250ZW50IjoiTFMwdExTMUNSVWRKVGlCRFJWSlVTVVpKUTBGVVJTMHRMUzB0Q2sxSlNVUjBha05EUVhwNVowRjNTVUpCWjBsVlJWUkpSREJFYUd0WFdFWndlSEFyWjBST2FFRkhkWGg1VFhOamQwTm5XVWxMYjFwSmVtb3dSVUYzVFhjS1RucEZWazFDVFVkQk1WVkZRMmhOVFdNeWJHNWpNMUoyWTIxVmRWcEhWakpOVWpSM1NFRlpSRlpSVVVSRmVGWjZZVmRrZW1SSE9YbGFVekZ3WW01U2JBcGpiVEZzV2tkc2FHUkhWWGRJYUdOT1RXcEplRTFVU1hsTlJFRjRUV3BOTlZkb1kwNU5ha2w0VFZSSmVVMUVRWGxOYWswMVYycEJRVTFHYTNkRmQxbElDa3R2V2tsNmFqQkRRVkZaU1V0dldrbDZhakJFUVZGalJGRm5RVVZzVGl0aU9DOUViemc0UVVzck5qSXJURlJFTWpkMk5EZEZVbXRwTkdweE5EQkZRMDRLV25NNWVFSTJRemwwZDFGaVlTOXFNeXR3VmtoMlpGWlJiMVZYZEdSR2FYTnBTbm80V0doNVQzcG5kMWhFVjNkR01UWlBRMEZzYzNkblowcFlUVUUwUndwQk1WVmtSSGRGUWk5M1VVVkJkMGxJWjBSQlZFSm5UbFpJVTFWRlJFUkJTMEpuWjNKQ1owVkdRbEZqUkVGNlFXUkNaMDVXU0ZFMFJVWm5VVlYwWVZSSUNuQjZXbkpsTW1kRFVEaDBVRlptYmpGb1JuVm1UMnhSZDBoM1dVUldVakJxUWtKbmQwWnZRVlV6T1ZCd2VqRlphMFZhWWpWeFRtcHdTMFpYYVhocE5Ga0tXa1E0ZDJKUldVUldVakJTUVZGSUwwSkhUWGRaV1ZwbVlVaFNNR05JVFRaTWVUbHVZVmhTYjJSWFNYVlpNamwwVERKT2IxbFhiSFZhTTFab1kyMVJkQXBoVnpGb1dqSldla3d5YUd4aVIzaDJURmhrZG1OdGVHdE1lVFZ1WVZoU2IyUlhTWFprTWpsNVlUSmFjMkl6WkhwTU0wcHNZa2RXYUdNeVZYVmxWMFowQ21KRlFubGFWMXA2VERKb2JGbFhVbnBNTWpGb1lWYzBkMDlSV1V0TGQxbENRa0ZIUkhaNlFVSkJVVkZ5WVVoU01HTklUVFpNZVRrd1lqSjBiR0pwTldnS1dUTlNjR0l5TlhwTWJXUndaRWRvTVZsdVZucGFXRXBxWWpJMU1GcFhOVEJNYlU1MllsUkJWMEpuYjNKQ1owVkZRVmxQTDAxQlJVTkNRV2g2V1RKb2JBcGFTRlp6V2xSQk1rSm5iM0pDWjBWRlFWbFBMMDFCUlVSQ1EyaHNUbTFOTTA1NlNYZFpWRWw1VG1wbk1rOUVVVE5QUjFFelRtMVJkMWw2WTNwT1JGbDVDazlFYXpCYVYwVjZXVmRPYUU1NldUTk5RbmRIUTJselIwRlJVVUpuTnpoM1FWRlJSVVJyVG5sYVYwWXdXbE5DVTFwWGVHeFpXRTVzVFVOelIwTnBjMGNLUVZGUlFtYzNPSGRCVVZWRlNGZE9iMWxYYkhWYU0xWm9ZMjFSZEdGWE1XaGFNbFo2VERKb2JHSkhlSFpNV0dSMlkyMTRhMDFDTUVkRGFYTkhRVkZSUWdwbk56aDNRVkZaUlVRelNteGFiazEyWVVkV2FGcElUWFppVjBad1ltcERRbWwzV1V0TGQxbENRa0ZJVjJWUlNVVkJaMUk1UWtoelFXVlJRak5CVGpBNUNrMUhja2Q0ZUVWNVdYaHJaVWhLYkc1T2QwdHBVMncyTkROcWVYUXZOR1ZMWTI5QmRrdGxOazlCUVVGQ2FFcDVkVUZFYTBGQlFWRkVRVVZuZDFKblNXZ0tRVXc0UjBnNVZHZFNSbWhhZFVwelRTdHlNbU0zVFVONk1HWkljeko0YldGcVZEbHdWakZoZGpOV1IzbEJhVVZCYkZWcldHSkhiSGxDUnpaWGFqVlBMd28zTDJwMWFVMXJRVW9yWmtaaWRWQlhjbTlzY1hWcWNXOXRTVlYzUTJkWlNVdHZXa2w2YWpCRlFYZE5SR0ZCUVhkYVVVbDNWM0JFYVZOeVNHODFWRlJKQ2l0MU1XTm5NWFowVEVScVp6UmhjemhNTUZOTk5FTjZlV3R4Ym1rNFZGcFRTV3hFVUdaQlFYTlVPRzlMZW5oc0swWlJSSGRCYWtWQkwzcG5OekJhUW5RS09EaENWVkpYTUZwa1RtaExZVVZaV1ZrMk4xVTBORWg1VjB4WldEa3ZUSFJ3V21KU01FWlNZMGxEU1N0aGJFSndZamczZVdkRWEwb0tMUzB0TFMxRlRrUWdRMFZTVkVsR1NVTkJWRVV0TFMwdExRbz0ifX19fQ==",
          "integratedTime": 1669075972,
          "logIndex": 7575886,
          "logID": "c0d23d6ad406973f9559f3ba2d1ca01f84147d8ffc5b8445c224f98b9591801d"
        }
      },
      "Issuer": "https://token.actions.githubusercontent.com",
      "Subject": "https://github.com/chainguard-images/hello-world/.github/workflows/release.yaml@refs/heads/main",
      "githubWorkflowName": "Create Release",
      "githubWorkflowRef": "refs/heads/main",
      "githubWorkflowRepository": "chainguard-images/hello-world",
      "githubWorkflowSha": "e6c7720a226868478d76d0c73462894ea3aca767",
      "githubWorkflowTrigger": "schedule",
      "run_attempt": "1",
      "run_id": "3519170847",
      "sha": "e6c7720a226868478d76d0c73462894ea3aca767"
    }
  }
]
```

You can verify that the image was built in Github Actions in this repository from the `Issuer` and `Subject` fields.
</details>

## Build

This image is built with [melange](https://github.com/chainguard-dev/melange) and [apko](https://github.com/chainguard-dev/apko).

