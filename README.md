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
| `latest` | `sha256:9e88b902690991d415dc14e9509b482cb5b8afb6719d6606a235b37ad9d06ae7`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:9e88b902690991d415dc14e9509b482cb5b8afb6719d6606a235b37ad9d06ae7) | `amd64` `arm64` `armv7` |



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
        "docker-manifest-digest": "sha256:9e88b902690991d415dc14e9509b482cb5b8afb6719d6606a235b37ad9d06ae7"
      },
      "type": "cosign container image signature"
    },
    "optional": {
      "1.3.6.1.4.1.57264.1.1": "https://token.actions.githubusercontent.com",
      "1.3.6.1.4.1.57264.1.2": "schedule",
      "1.3.6.1.4.1.57264.1.3": "323a08959e4958d95b7b994c5d92460a4e628476",
      "1.3.6.1.4.1.57264.1.4": "Create Release",
      "1.3.6.1.4.1.57264.1.5": "chainguard-images/hello-world",
      "1.3.6.1.4.1.57264.1.6": "refs/heads/main",
      "Bundle": {
        "SignedEntryTimestamp": "MEUCIQC40jjBHLIKL+CctBWlhBI3IIVL0BP0QbpX6WilZO1KLQIgX8P3axDKjdbp0lom7/EBbTup9qYiBz/HYjHj+C4eksw=",
        "Payload": {
          "body": "eyJhcGlWZXJzaW9uIjoiMC4wLjEiLCJraW5kIjoiaGFzaGVkcmVrb3JkIiwic3BlYyI6eyJkYXRhIjp7Imhhc2giOnsiYWxnb3JpdGhtIjoic2hhMjU2IiwidmFsdWUiOiIwNzk5OGQ5ZTkzYmIyZjQxODFhZTFiMzQ4OTgxZTVjODhjNWNlZmQxOGU3YmI2NjVlMjI3ZjUwYTI5MDMyZGJhIn19LCJzaWduYXR1cmUiOnsiY29udGVudCI6Ik1FUUNJQU55TzZQSnN5OEppR3pLbG9jNG9qY3EzUlBaUWRHTzdoOVlYMFpPK2Z5ZkFpQjNFb2w1WkJnMGFHT3lFcXVJblRoaDlXb0tXSnppZFBsTUhzRFdzZm9QYWc9PSIsInB1YmxpY0tleSI6eyJjb250ZW50IjoiTFMwdExTMUNSVWRKVGlCRFJWSlVTVVpKUTBGVVJTMHRMUzB0Q2sxSlNVUjBSRU5EUVhwMVowRjNTVUpCWjBsVlRHRk9SRkZEWkVsUGRIZGFNVk16YlhORmR6SXlObE4wU2xVMGQwTm5XVWxMYjFwSmVtb3dSVUYzVFhjS1RucEZWazFDVFVkQk1WVkZRMmhOVFdNeWJHNWpNMUoyWTIxVmRWcEhWakpOVWpSM1NFRlpSRlpSVVVSRmVGWjZZVmRrZW1SSE9YbGFVekZ3WW01U2JBcGpiVEZzV2tkc2FHUkhWWGRJYUdOT1RXcEplRTFVU1hwTlJFRjRUV3BOTlZkb1kwNU5ha2w0VFZSSmVrMUVRWGxOYWswMVYycEJRVTFHYTNkRmQxbElDa3R2V2tsNmFqQkRRVkZaU1V0dldrbDZhakJFUVZGalJGRm5RVVZaZW1seE5WZDZNVmcyUTNkR05UaG5WRXBxZFRkbWVFZGhRMEpDVGxoWE1IZENiRVVLYld0VVRXSjBibFJVTld4ME5rOXNaMlYzUjJkQlJIcEpTVmszWTJrclkxZEVLMjV4WVZJMU5GQm1SMUZMZWpjeVkzRlBRMEZzYjNkblowcFhUVUUwUndwQk1WVmtSSGRGUWk5M1VVVkJkMGxJWjBSQlZFSm5UbFpJVTFWRlJFUkJTMEpuWjNKQ1owVkdRbEZqUkVGNlFXUkNaMDVXU0ZFMFJVWm5VVlUwY1RCUUNqZEdTMEUwYWpSaVFXUjJUbkIyYmtSeGRWTjNOMmR6ZDBoM1dVUldVakJxUWtKbmQwWnZRVlV6T1ZCd2VqRlphMFZhWWpWeFRtcHdTMFpYYVhocE5Ga0tXa1E0ZDJKUldVUldVakJTUVZGSUwwSkhUWGRaV1ZwbVlVaFNNR05JVFRaTWVUbHVZVmhTYjJSWFNYVlpNamwwVERKT2IxbFhiSFZhTTFab1kyMVJkQXBoVnpGb1dqSldla3d5YUd4aVIzaDJURmhrZG1OdGVHdE1lVFZ1WVZoU2IyUlhTWFprTWpsNVlUSmFjMkl6WkhwTU0wcHNZa2RXYUdNeVZYVmxWMFowQ21KRlFubGFWMXA2VERKb2JGbFhVbnBNTWpGb1lWYzBkMDlSV1V0TGQxbENRa0ZIUkhaNlFVSkJVVkZ5WVVoU01HTklUVFpNZVRrd1lqSjBiR0pwTldnS1dUTlNjR0l5TlhwTWJXUndaRWRvTVZsdVZucGFXRXBxWWpJMU1GcFhOVEJNYlU1MllsUkJWMEpuYjNKQ1owVkZRVmxQTDAxQlJVTkNRV2g2V1RKb2JBcGFTRlp6V2xSQk1rSm5iM0pDWjBWRlFWbFBMMDFCUlVSQ1EyZDZUV3BPYUUxRVp6Vk9WR3hzVGtSck1VOUhVVFZPVjBreldXcHJOVTVIVFRGYVJHdDVDazVFV1hkWlZGSnNUbXBKTkU1RVl6Sk5RbmRIUTJselIwRlJVVUpuTnpoM1FWRlJSVVJyVG5sYVYwWXdXbE5DVTFwWGVHeFpXRTVzVFVOelIwTnBjMGNLUVZGUlFtYzNPSGRCVVZWRlNGZE9iMWxYYkhWYU0xWm9ZMjFSZEdGWE1XaGFNbFo2VERKb2JHSkhlSFpNV0dSMlkyMTRhMDFDTUVkRGFYTkhRVkZSUWdwbk56aDNRVkZaUlVRelNteGFiazEyWVVkV2FGcElUWFppVjBad1ltcERRbWxuV1V0TGQxbENRa0ZJVjJWUlNVVkJaMUk0UWtodlFXVkJRakpCVGpBNUNrMUhja2Q0ZUVWNVdYaHJaVWhLYkc1T2QwdHBVMncyTkROcWVYUXZOR1ZMWTI5QmRrdGxOazlCUVVGQ2FFdElWVmRvYzBGQlFWRkVRVVZqZDFKUlNXY0tUbXhKVDA5UllWRXpiMjFGYXpsMGEzUXhZbEZ5TUUxMlEwTnhhVzlSZDIwd1FqRlFRM2xpTmxRNU1FTkpVVVJ3YkdKUk16RlJVMFEyTldOWE0yMXpNZ292WVRVNU1tVjBiM0I1Y3k5T1EzUllOM00xUzJwQldHVXJSRUZMUW1kbmNXaHJhazlRVVZGRVFYZE9ia0ZFUW10QmFrRkZUMEZXVTBsMldGVnNiWGRqQ2pSMGRubHljbkY1SzNsQ1RXMXNOVmxXYUdNMllVNWFWQ3QyUTFaUWFYZHdkSEoyZDNoWVl5dGljbTVCTUd0RUszcGlZME5OU0ROUWFXaFRRMFZxSzBvS1NUTnNTMUJaU0VwMWRWbzRiR3R6UlcxMU5tWk5PVFZUY0ZFMllXczViRGxXTUcxeGR6ZEtORUYzUzBkWkx6SnlUa3BISzBSM1BUMEtMUzB0TFMxRlRrUWdRMFZTVkVsR1NVTkJWRVV0TFMwdExRbz0ifX19fQ==",
          "integratedTime": 1669162369,
          "logIndex": 7651500,
          "logID": "c0d23d6ad406973f9559f3ba2d1ca01f84147d8ffc5b8445c224f98b9591801d"
        }
      },
      "Issuer": "https://token.actions.githubusercontent.com",
      "Subject": "https://github.com/chainguard-images/hello-world/.github/workflows/release.yaml@refs/heads/main",
      "githubWorkflowName": "Create Release",
      "githubWorkflowRef": "refs/heads/main",
      "githubWorkflowRepository": "chainguard-images/hello-world",
      "githubWorkflowSha": "323a08959e4958d95b7b994c5d92460a4e628476",
      "githubWorkflowTrigger": "schedule",
      "run_attempt": "1",
      "run_id": "3528104772",
      "sha": "323a08959e4958d95b7b994c5d92460a4e628476"
    }
  }
]
```

You can verify that the image was built in Github Actions in this repository from the `Issuer` and `Subject` fields.
</details>

## Build

This image is built with [melange](https://github.com/chainguard-dev/melange) and [apko](https://github.com/chainguard-dev/apko).

