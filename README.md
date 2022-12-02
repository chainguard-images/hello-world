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
| `latest` | `sha256:0c15ef1bb64bd82ff0bd6c1c5968d5b1daabc1f1f234e503ebbb41ae786231ef`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:0c15ef1bb64bd82ff0bd6c1c5968d5b1daabc1f1f234e503ebbb41ae786231ef) | `amd64` `arm64` `armv7` |



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
        "docker-manifest-digest": "sha256:0c15ef1bb64bd82ff0bd6c1c5968d5b1daabc1f1f234e503ebbb41ae786231ef"
      },
      "type": "cosign container image signature"
    },
    "optional": {
      "1.3.6.1.4.1.57264.1.1": "https://token.actions.githubusercontent.com",
      "1.3.6.1.4.1.57264.1.2": "schedule",
      "1.3.6.1.4.1.57264.1.3": "dfa02572a041849f2a1ca9c8f6a99bd6e567b107",
      "1.3.6.1.4.1.57264.1.4": "Create Release",
      "1.3.6.1.4.1.57264.1.5": "chainguard-images/hello-world",
      "1.3.6.1.4.1.57264.1.6": "refs/heads/main",
      "Bundle": {
        "SignedEntryTimestamp": "MEUCIQDfub6tB0VEFcsEOdnO9H51YqibFu5RPKVXJkBbRZCAmgIgVSUNwurEUbbYRFQhdWIfSWxd5NYJP+V5FqyCsa2o8y4=",
        "Payload": {
          "body": "eyJhcGlWZXJzaW9uIjoiMC4wLjEiLCJraW5kIjoiaGFzaGVkcmVrb3JkIiwic3BlYyI6eyJkYXRhIjp7Imhhc2giOnsiYWxnb3JpdGhtIjoic2hhMjU2IiwidmFsdWUiOiJlN2QwMjRiMjNlMWU2NjZmMGZkOTIwZDNkZWViYWUxMDYwY2E5NDQyYjk5ZDYzYWI3MTdkNmRlMGRkNTI1NmFjIn19LCJzaWduYXR1cmUiOnsiY29udGVudCI6Ik1FVUNJUURHSmxLb0NJTGF5RFU4UzhVZkl5QkFjYzJNeWZjbTZZd1ZadE43ZHQyWTRBSWdaRGl2ZTNjWmdXNmhTZFJCZ3FpOHV6T3dOVTlJTDJxdXBEZkdTcDBLcm1NPSIsInB1YmxpY0tleSI6eyJjb250ZW50IjoiTFMwdExTMUNSVWRKVGlCRFJWSlVTVVpKUTBGVVJTMHRMUzB0Q2sxSlNVUjBSRU5EUVhweFowRjNTVUpCWjBsVlduWnVVMkZVWTBWTmNUVnhkVWx4TkRKMFVYRkhNRGcyVUdKbmQwTm5XVWxMYjFwSmVtb3dSVUYzVFhjS1RucEZWazFDVFVkQk1WVkZRMmhOVFdNeWJHNWpNMUoyWTIxVmRWcEhWakpOVWpSM1NFRlpSRlpSVVVSRmVGWjZZVmRrZW1SSE9YbGFVekZ3WW01U2JBcGpiVEZzV2tkc2FHUkhWWGRJYUdOT1RXcEplRTFxUVhsTlJFRjRUVlJCZVZkb1kwNU5ha2w0VFdwQmVVMUVRWGxOVkVGNVYycEJRVTFHYTNkRmQxbElDa3R2V2tsNmFqQkRRVkZaU1V0dldrbDZhakJFUVZGalJGRm5RVVZZVEd4UmRsRlZVMEkwYUhaRE5uZGpVa1p5ZDBob2VXdHpkbXhGWms5eGIyeEdiVGtLSzJ3elZXOW9jbk56U25aRFlqRkhTVE5oU0hFek0ya3ljRFJuZEcxMFJHMXlUMlIyY1ROcWExbFVVa2wxU0ZRMFZIRlBRMEZzYTNkblowcFdUVUUwUndwQk1WVmtSSGRGUWk5M1VVVkJkMGxJWjBSQlZFSm5UbFpJVTFWRlJFUkJTMEpuWjNKQ1owVkdRbEZqUkVGNlFXUkNaMDVXU0ZFMFJVWm5VVlZGYml0akNpc3ZUMmhzTldWQlNrMURSbUoyTW5OV1dYRnJSVFF3ZDBoM1dVUldVakJxUWtKbmQwWnZRVlV6T1ZCd2VqRlphMFZhWWpWeFRtcHdTMFpYYVhocE5Ga0tXa1E0ZDJKUldVUldVakJTUVZGSUwwSkhUWGRaV1ZwbVlVaFNNR05JVFRaTWVUbHVZVmhTYjJSWFNYVlpNamwwVERKT2IxbFhiSFZhTTFab1kyMVJkQXBoVnpGb1dqSldla3d5YUd4aVIzaDJURmhrZG1OdGVHdE1lVFZ1WVZoU2IyUlhTWFprTWpsNVlUSmFjMkl6WkhwTU0wcHNZa2RXYUdNeVZYVmxWMFowQ21KRlFubGFWMXA2VERKb2JGbFhVbnBNTWpGb1lWYzBkMDlSV1V0TGQxbENRa0ZIUkhaNlFVSkJVVkZ5WVVoU01HTklUVFpNZVRrd1lqSjBiR0pwTldnS1dUTlNjR0l5TlhwTWJXUndaRWRvTVZsdVZucGFXRXBxWWpJMU1GcFhOVEJNYlU1MllsUkJWMEpuYjNKQ1owVkZRVmxQTDAxQlJVTkNRV2g2V1RKb2JBcGFTRlp6V2xSQk1rSm5iM0pDWjBWRlFWbFBMMDFCUlVSQ1EyaHJXbTFGZDAxcVZUTk5iVVYzVGtSRk5FNUViRzFOYlVWNFdUSkZOVmw2YUcxT2JVVTFDazlYU210T2JWVXhUbXBrYVUxVVFUTk5RbmRIUTJselIwRlJVVUpuTnpoM1FWRlJSVVJyVG5sYVYwWXdXbE5DVTFwWGVHeFpXRTVzVFVOelIwTnBjMGNLUVZGUlFtYzNPSGRCVVZWRlNGZE9iMWxYYkhWYU0xWm9ZMjFSZEdGWE1XaGFNbFo2VERKb2JHSkhlSFpNV0dSMlkyMTRhMDFDTUVkRGFYTkhRVkZSUWdwbk56aDNRVkZaUlVRelNteGFiazEyWVVkV2FGcElUWFppVjBad1ltcERRbWxSV1V0TGQxbENRa0ZJVjJWUlNVVkJaMUkzUWtoclFXUjNRakZCVGpBNUNrMUhja2Q0ZUVWNVdYaHJaVWhLYkc1T2QwdHBVMncyTkROcWVYUXZOR1ZMWTI5QmRrdGxOazlCUVVGQ2FFNUJjMGhFYjBGQlFWRkVRVVZaZDFKQlNXY0tTV3BCYnpJelVFMDFkRGxPT0daMk5VUXZjMnRQVlN0UEszRmhOMDFqWVhGTVJFZDNiVmR2YVRkSlVVTkpRVlp6VDFBMlJUWkpUakZ0YzA1Q2JsUkNVQXBwYlZWbWFVcHlNRk5NZUZRMmJFTXZZa0p6ZURoeFNHWk5RVzlIUTBOeFIxTk5ORGxDUVUxRVFUSm5RVTFIVlVOTlVVTndUMkl2VlhGVVNFeHZlWHBMQ2tGNFptWk1VMlJ5UkZWUlZEaDVWU3RVZDNSdVMxZElUblJxYTFGd09WbDNXQzlUT0hOSFRISXlha2RDYVdKdGVFVlJSVU5OUkhKVFlsZ3djMGhXZEVvS1JVVjVUM2h5WW5KMWQxaFlNMVJFZURJMFNUY3JkMWhQTlVjdlREVTJjVVZOZWpWU1ZGWTJUa1UwWTNCelVpdGtZbXhUY1hCUlBUMEtMUzB0TFMxRlRrUWdRMFZTVkVsR1NVTkJWRVV0TFMwdExRbz0ifX19fQ==",
          "integratedTime": 1669939874,
          "logIndex": 8258345,
          "logID": "c0d23d6ad406973f9559f3ba2d1ca01f84147d8ffc5b8445c224f98b9591801d"
        }
      },
      "Issuer": "https://token.actions.githubusercontent.com",
      "Subject": "https://github.com/chainguard-images/hello-world/.github/workflows/release.yaml@refs/heads/main",
      "githubWorkflowName": "Create Release",
      "githubWorkflowRef": "refs/heads/main",
      "githubWorkflowRepository": "chainguard-images/hello-world",
      "githubWorkflowSha": "dfa02572a041849f2a1ca9c8f6a99bd6e567b107",
      "githubWorkflowTrigger": "schedule",
      "run_attempt": "1",
      "run_id": "3597642840",
      "sha": "dfa02572a041849f2a1ca9c8f6a99bd6e567b107"
    }
  }
]
```

You can verify that the image was built in Github Actions in this repository from the `Issuer` and `Subject` fields.
</details>

## Build

This image is built with [melange](https://github.com/chainguard-dev/melange) and [apko](https://github.com/chainguard-dev/apko).

