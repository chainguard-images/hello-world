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
| `latest` | `sha256:d61136b13c999478f80e7f55c811cf28a5bc09fbe1809d4ff42c34d23aac9c57`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:d61136b13c999478f80e7f55c811cf28a5bc09fbe1809d4ff42c34d23aac9c57) | `amd64` `arm64` `armv7` |



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
        "docker-manifest-digest": "sha256:d61136b13c999478f80e7f55c811cf28a5bc09fbe1809d4ff42c34d23aac9c57"
      },
      "type": "cosign container image signature"
    },
    "optional": {
      "1.3.6.1.4.1.57264.1.1": "https://token.actions.githubusercontent.com",
      "1.3.6.1.4.1.57264.1.2": "schedule",
      "1.3.6.1.4.1.57264.1.3": "b9384d26984fc888f4d0a4ebda027e224cb86f1e",
      "1.3.6.1.4.1.57264.1.4": "Create Release",
      "1.3.6.1.4.1.57264.1.5": "chainguard-images/hello-world",
      "1.3.6.1.4.1.57264.1.6": "refs/heads/main",
      "Bundle": {
        "SignedEntryTimestamp": "MEUCIQDUxWZLfGPnQsAG2U4FrUiYtZDmRfCf0yqlTwYjbChOFgIgVplXIIbF5MBPK7AoU95gim9+NXf0lD/RX9NLt3jQyFY=",
        "Payload": {
          "body": "eyJhcGlWZXJzaW9uIjoiMC4wLjEiLCJraW5kIjoiaGFzaGVkcmVrb3JkIiwic3BlYyI6eyJkYXRhIjp7Imhhc2giOnsiYWxnb3JpdGhtIjoic2hhMjU2IiwidmFsdWUiOiJlNTcyZWMxYzY1YzUwNTYyOTljN2Q1ZTFkMDc3NjAyNzY3MWUxYzEwMzNiMWU4NTNkMGY4MTdjZWY1MzQzMGIwIn19LCJzaWduYXR1cmUiOnsiY29udGVudCI6Ik1FWUNJUURiR2JmYkhLZmoxSHlhUEpoWHJabHRldHBSdVl6c0VyNWxrV2g2VHJkVW1nSWhBTU9md3I1VEFXL1hiZmI0L05sd2NJbks0VUNhQWF5WEovQ2JWMlNETTJuMCIsInB1YmxpY0tleSI6eyJjb250ZW50IjoiTFMwdExTMUNSVWRKVGlCRFJWSlVTVVpKUTBGVVJTMHRMUzB0Q2sxSlNVUjBSRU5EUVhwMVowRjNTVUpCWjBsVlZDdEpaSHBwTkZOMFlrNTJZMDkwVGxjeVpYUnFkbmREY0V0UmQwTm5XVWxMYjFwSmVtb3dSVUYzVFhjS1RucEZWazFDVFVkQk1WVkZRMmhOVFdNeWJHNWpNMUoyWTIxVmRWcEhWakpOVWpSM1NFRlpSRlpSVVVSRmVGWjZZVmRrZW1SSE9YbGFVekZ3WW01U2JBcGpiVEZzV2tkc2FHUkhWWGRJYUdOT1RXcEplRTFVU1ROTlJFRjRUV3BSZVZkb1kwNU5ha2w0VFZSSk0wMUVRWGxOYWxGNVYycEJRVTFHYTNkRmQxbElDa3R2V2tsNmFqQkRRVkZaU1V0dldrbDZhakJFUVZGalJGRm5RVVZGZUhseGJXUXpNRlV2VURKc2NXbDVaRnBIV25WeVVsWjNRa3AzV0VKUE4wNUlSRU1LVlU5elZUTlZRblJCV21ReGRXTXhjVFk0YlV4aFIxVmxZWGd4UTBaTVYwRjJjQ3R2WkVNMGNXTXpSMEV4V0RoUE5rdFBRMEZzYjNkblowcFhUVUUwUndwQk1WVmtSSGRGUWk5M1VVVkJkMGxJWjBSQlZFSm5UbFpJVTFWRlJFUkJTMEpuWjNKQ1owVkdRbEZqUkVGNlFXUkNaMDVXU0ZFMFJVWm5VVlZ5WjNSM0NreHVSemRtYzNscGRtWndlVk5NVHpWaloybGthMWRKZDBoM1dVUldVakJxUWtKbmQwWnZRVlV6T1ZCd2VqRlphMFZhWWpWeFRtcHdTMFpYYVhocE5Ga0tXa1E0ZDJKUldVUldVakJTUVZGSUwwSkhUWGRaV1ZwbVlVaFNNR05JVFRaTWVUbHVZVmhTYjJSWFNYVlpNamwwVERKT2IxbFhiSFZhTTFab1kyMVJkQXBoVnpGb1dqSldla3d5YUd4aVIzaDJURmhrZG1OdGVHdE1lVFZ1WVZoU2IyUlhTWFprTWpsNVlUSmFjMkl6WkhwTU0wcHNZa2RXYUdNeVZYVmxWMFowQ21KRlFubGFWMXA2VERKb2JGbFhVbnBNTWpGb1lWYzBkMDlSV1V0TGQxbENRa0ZIUkhaNlFVSkJVVkZ5WVVoU01HTklUVFpNZVRrd1lqSjBiR0pwTldnS1dUTlNjR0l5TlhwTWJXUndaRWRvTVZsdVZucGFXRXBxWWpJMU1GcFhOVEJNYlU1MllsUkJWMEpuYjNKQ1owVkZRVmxQTDAxQlJVTkNRV2g2V1RKb2JBcGFTRlp6V2xSQk1rSm5iM0pDWjBWRlFWbFBMMDFCUlVSQ1EyaHBUMVJOTkU1SFVYbE9hbXMwVGtkYWFrOUVaelJhYWxKclRVZEZNRnBYU210WlZFRjVDazR5VlhsTmFsSnFXV3BuTWxwcVJteE5RbmRIUTJselIwRlJVVUpuTnpoM1FWRlJSVVJyVG5sYVYwWXdXbE5DVTFwWGVHeFpXRTVzVFVOelIwTnBjMGNLUVZGUlFtYzNPSGRCVVZWRlNGZE9iMWxYYkhWYU0xWm9ZMjFSZEdGWE1XaGFNbFo2VERKb2JHSkhlSFpNV0dSMlkyMTRhMDFDTUVkRGFYTkhRVkZSUWdwbk56aDNRVkZaUlVRelNteGFiazEyWVVkV2FGcElUWFppVjBad1ltcERRbWxuV1V0TGQxbENRa0ZJVjJWUlNVVkJaMUk0UWtodlFXVkJRakpCVGpBNUNrMUhja2Q0ZUVWNVdYaHJaVWhLYkc1T2QwdHBVMncyTkROcWVYUXZOR1ZMWTI5QmRrdGxOazlCUVVGQ2FFeGFkREV6TkVGQlFWRkVRVVZqZDFKUlNXY0tRV3MzVDFWSk15dGpielJaT0dGWlprWm5WMFJ6ZDA5bUsyTlFaMDVIY1M5WmNreDBUMVZ4WWs1VFowTkpVVVFyUjNaRFlVbDBhWEpPVW1GTVQwdG1kd3B3Y1M5aUx6RjVVVEJwZDNCd1lXRTJVVXQxZDNoa2QybHFla0ZMUW1kbmNXaHJhazlRVVZGRVFYZE9ia0ZFUW10QmFrRlNSVU5HYVd0SE0xUmFXbFFyQ2xabmR6QjBNM05tUzBSaFVVZFhURkprZG1aYU9GcGhRa2RXWVhKWFVrbElMMFoxY0ZkNmQwUkdNMmhXT1VjMU4xbFFiME5OUnpGVmMwVm9abTlXU0ZrS2RuQnFUM3BtYzB4dlZrdEtVRWxSV1ROVWIzaDVkM1ZHY205RlFUQnFSR1J2WjJaR1lXUllNemh2YkdwRVlYQkVURlUxYkc1blBUMEtMUzB0TFMxRlRrUWdRMFZTVkVsR1NVTkJWRVV0TFMwdExRbz0ifX19fQ==",
          "integratedTime": 1669507972,
          "logIndex": 7917216,
          "logID": "c0d23d6ad406973f9559f3ba2d1ca01f84147d8ffc5b8445c224f98b9591801d"
        }
      },
      "Issuer": "https://token.actions.githubusercontent.com",
      "Subject": "https://github.com/chainguard-images/hello-world/.github/workflows/release.yaml@refs/heads/main",
      "githubWorkflowName": "Create Release",
      "githubWorkflowRef": "refs/heads/main",
      "githubWorkflowRepository": "chainguard-images/hello-world",
      "githubWorkflowSha": "b9384d26984fc888f4d0a4ebda027e224cb86f1e",
      "githubWorkflowTrigger": "schedule",
      "run_attempt": "1",
      "run_id": "3555931233",
      "sha": "b9384d26984fc888f4d0a4ebda027e224cb86f1e"
    }
  }
]
```

You can verify that the image was built in Github Actions in this repository from the `Issuer` and `Subject` fields.
</details>

## Build

This image is built with [melange](https://github.com/chainguard-dev/melange) and [apko](https://github.com/chainguard-dev/apko).

