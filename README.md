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
| `latest` | `sha256:54602b2e8bacc9264c29de581a4258daf3534b1e70a5918587ff721fd6fa8821`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:54602b2e8bacc9264c29de581a4258daf3534b1e70a5918587ff721fd6fa8821) | `amd64` `arm64` `armv7` |



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
        "docker-manifest-digest": "sha256:54602b2e8bacc9264c29de581a4258daf3534b1e70a5918587ff721fd6fa8821"
      },
      "type": "cosign container image signature"
    },
    "optional": {
      "1.3.6.1.4.1.57264.1.1": "https://token.actions.githubusercontent.com",
      "1.3.6.1.4.1.57264.1.2": "schedule",
      "1.3.6.1.4.1.57264.1.3": "dd2cc53be1a9f6130b5734a9131ddd0f2fe7c546",
      "1.3.6.1.4.1.57264.1.4": "Create Release",
      "1.3.6.1.4.1.57264.1.5": "chainguard-images/hello-world",
      "1.3.6.1.4.1.57264.1.6": "refs/heads/main",
      "Bundle": {
        "SignedEntryTimestamp": "MEYCIQCZg/TPacBit0rQhVlvS+RP1QwZyrw2/KpOcBSD2VfaJwIhAKbcGOvunDF1D0AFzpiwHBlt1RYUN1K9zrbPFkxEvH0G",
        "Payload": {
          "body": "eyJhcGlWZXJzaW9uIjoiMC4wLjEiLCJraW5kIjoiaGFzaGVkcmVrb3JkIiwic3BlYyI6eyJkYXRhIjp7Imhhc2giOnsiYWxnb3JpdGhtIjoic2hhMjU2IiwidmFsdWUiOiJiMGJkZDAyY2E5ZDUwNDBkMmVjYmFmM2YzYzg5NjZlYzA2ZDEyNjhkOWU5ZTk4MDkwZmZhYWU3NDRjYTNhYWVmIn19LCJzaWduYXR1cmUiOnsiY29udGVudCI6Ik1FWUNJUUQzcE1RQ1orVW9Xb0l5T2Vja1lUcEIyRDg1RGVrWE82Tk5HbXl1dHRodGJRSWhBS1M4RzRVVzYzYy9UT1BVamZMNkFkdEdxYnBleThWWjd0OGIxc29mNFFYNSIsInB1YmxpY0tleSI6eyJjb250ZW50IjoiTFMwdExTMUNSVWRKVGlCRFJWSlVTVVpKUTBGVVJTMHRMUzB0Q2sxSlNVUjBSRU5EUVhwMVowRjNTVUpCWjBsVlFtRkdOelpNZEhsRlZHUjZPVkZzU0dwU1FVSlVWbFE1Y25CTmQwTm5XVWxMYjFwSmVtb3dSVUYzVFhjS1RucEZWazFDVFVkQk1WVkZRMmhOVFdNeWJHNWpNMUoyWTIxVmRWcEhWakpOVWpSM1NFRlpSRlpSVVVSRmVGWjZZVmRrZW1SSE9YbGFVekZ3WW01U2JBcGpiVEZzV2tkc2FHUkhWWGRJYUdOT1RXcEplRTFFVFhoTlJFVjVUVVJOZVZkb1kwNU5ha2w0VFVSTmVFMUVSWHBOUkUxNVYycEJRVTFHYTNkRmQxbElDa3R2V2tsNmFqQkRRVkZaU1V0dldrbDZhakJFUVZGalJGRm5RVVY0T1ZVMFMyTk5iMEZ4TVdsWFZHUlZaVEpVTld4d2JXWlZXVkkwUW1jdmJpdGhSRmNLZG5WNE5HdGxUQzlFYW5oc1ZteDNhR2t4VFZGelJuRkpaRk56UTJ4bVZDOU9UbkpEUVRKM1EyWkNSekF6WTNwelNrdFBRMEZzYjNkblowcFhUVUUwUndwQk1WVmtSSGRGUWk5M1VVVkJkMGxJWjBSQlZFSm5UbFpJVTFWRlJFUkJTMEpuWjNKQ1owVkdRbEZqUkVGNlFXUkNaMDVXU0ZFMFJVWm5VVlZGWVRVMUNuQnNUeXRaU0VadGVVeG9iVkpRYWs1bE5YTnZUbG8wZDBoM1dVUldVakJxUWtKbmQwWnZRVlV6T1ZCd2VqRlphMFZhWWpWeFRtcHdTMFpYYVhocE5Ga0tXa1E0ZDJKUldVUldVakJTUVZGSUwwSkhUWGRaV1ZwbVlVaFNNR05JVFRaTWVUbHVZVmhTYjJSWFNYVlpNamwwVERKT2IxbFhiSFZhTTFab1kyMVJkQXBoVnpGb1dqSldla3d5YUd4aVIzaDJURmhrZG1OdGVHdE1lVFZ1WVZoU2IyUlhTWFprTWpsNVlUSmFjMkl6WkhwTU0wcHNZa2RXYUdNeVZYVmxWMFowQ21KRlFubGFWMXA2VERKb2JGbFhVbnBNTWpGb1lWYzBkMDlSV1V0TGQxbENRa0ZIUkhaNlFVSkJVVkZ5WVVoU01HTklUVFpNZVRrd1lqSjBiR0pwTldnS1dUTlNjR0l5TlhwTWJXUndaRWRvTVZsdVZucGFXRXBxWWpJMU1GcFhOVEJNYlU1MllsUkJWMEpuYjNKQ1owVkZRVmxQTDAxQlJVTkNRV2g2V1RKb2JBcGFTRlp6V2xSQk1rSm5iM0pDWjBWRlFWbFBMMDFCUlVSQ1EyaHJXa1JLYWxsNlZYcFpiVlY0V1ZSc2JVNXFSWHBOUjBreFRucE5NRmxVYTNoTmVrWnJDbHBIVVhkYWFrcHRXbFJrYWs1VVVUSk5RbmRIUTJselIwRlJVVUpuTnpoM1FWRlJSVVJyVG5sYVYwWXdXbE5DVTFwWGVHeFpXRTVzVFVOelIwTnBjMGNLUVZGUlFtYzNPSGRCVVZWRlNGZE9iMWxYYkhWYU0xWm9ZMjFSZEdGWE1XaGFNbFo2VERKb2JHSkhlSFpNV0dSMlkyMTRhMDFDTUVkRGFYTkhRVkZSUWdwbk56aDNRVkZaUlVRelNteGFiazEyWVVkV2FGcElUWFppVjBad1ltcERRbWxuV1V0TGQxbENRa0ZJVjJWUlNVVkJaMUk0UWtodlFXVkJRakpCUVdobkNtdDJRVzlWZGpsdlVtUklVbUY1WlVWdVJWWnVSMHQzVjFCalRUUXdiVE50ZGtOSlIwNXRPWGxCUVVGQ2FFTjFaMUJLYTBGQlFWRkVRVVZqZDFKUlNXY0taRzR5WW1nd1ZrTm5OMjVpTVZOeWJtaDJRMWwwYlVSUlZHdFhTVkYzYVRGaFRWZFRTRVV4ZHpsNmEwTkpVVVJZWVZOeFIxRjZZWEphT0VkUWJrUXdVd3BGWVVZeVNFRktabXBUY1ZWTGJHSkpaVmxLVG1oTFMyaE1WRUZMUW1kbmNXaHJhazlRVVZGRVFYZE9ia0ZFUW10QmFrRllhakpCUkdONE1GUlRTSGh5Q2s1NVpXTkdlREExZVV4alZrVjJaR3h4VTNWdVNXdHpiM1o1UzI1VWIxTXhjQzlpU25Bd1kyVm9ZVVJFYzFVeVJFNHlRVU5OUlVOeFdXOXZXRmd4UzNFS1VVdHhkR0l3ZHpCWVYwUklOME5vYVU5NVEyWlhTRmRRT1hkdFltNVBhVlZ5YjBoVFRVMHdPR2RITkRsVGJFTnFVbTlVTXpablBUMEtMUzB0TFMxRlRrUWdRMFZTVkVsR1NVTkJWRVV0TFMwdExRbz0ifX19fQ==",
          "integratedTime": 1667179240,
          "logIndex": 6191133,
          "logID": "c0d23d6ad406973f9559f3ba2d1ca01f84147d8ffc5b8445c224f98b9591801d"
        }
      },
      "Issuer": "https://token.actions.githubusercontent.com",
      "Subject": "https://github.com/chainguard-images/hello-world/.github/workflows/release.yaml@refs/heads/main",
      "githubWorkflowName": "Create Release",
      "githubWorkflowRef": "refs/heads/main",
      "githubWorkflowRepository": "chainguard-images/hello-world",
      "githubWorkflowSha": "dd2cc53be1a9f6130b5734a9131ddd0f2fe7c546",
      "githubWorkflowTrigger": "schedule",
      "run_attempt": "1",
      "run_id": "3357868421",
      "sha": "dd2cc53be1a9f6130b5734a9131ddd0f2fe7c546"
    }
  }
]
```

You can verify that the image was built in Github Actions in this repository from the `Issuer` and `Subject` fields.
</details>

## Build

This image is built with [melange](https://github.com/chainguard-dev/melange) and [apko](https://github.com/chainguard-dev/apko).

