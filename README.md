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
| `latest` | `sha256:cd8a60ffb1a4158f12808edb3a1176145bc889e4adeed2c12155c74694088c06`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:cd8a60ffb1a4158f12808edb3a1176145bc889e4adeed2c12155c74694088c06) | `amd64` `arm64` `armv7` |



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
        "docker-manifest-digest": "sha256:cd8a60ffb1a4158f12808edb3a1176145bc889e4adeed2c12155c74694088c06"
      },
      "type": "cosign container image signature"
    },
    "optional": {
      "1.3.6.1.4.1.57264.1.1": "https://token.actions.githubusercontent.com",
      "1.3.6.1.4.1.57264.1.2": "schedule",
      "1.3.6.1.4.1.57264.1.3": "b3176c277e31494aa962662485b179b874d58a61",
      "1.3.6.1.4.1.57264.1.4": "Create Release",
      "1.3.6.1.4.1.57264.1.5": "chainguard-images/hello-world",
      "1.3.6.1.4.1.57264.1.6": "refs/heads/main",
      "Bundle": {
        "SignedEntryTimestamp": "MEYCIQD0DXxKRhvXblJNAakItze6YWCBGWEji4uXxF4tYnhW2QIhAMnU7rocacq9g+ghW5GkPf8BJoCZIJeFWptv1n2gO3f5",
        "Payload": {
          "body": "eyJhcGlWZXJzaW9uIjoiMC4wLjEiLCJraW5kIjoiaGFzaGVkcmVrb3JkIiwic3BlYyI6eyJkYXRhIjp7Imhhc2giOnsiYWxnb3JpdGhtIjoic2hhMjU2IiwidmFsdWUiOiI5ZWUwNmY4YjhkMzA2M2ZmYWZiNzdiNDRjNjM4ZjIwNmEyOThjYTg2OTNlN2RlYzgxMTIxNWEzY2M4NTI2MzA5In19LCJzaWduYXR1cmUiOnsiY29udGVudCI6Ik1FVUNJQlZ0RzlnbUdLc1lTa3NYcVpxb1FhRmVwOWtCQzJIS3dWRjZaNlBqUWxackFpRUFuOE9paEgwYkZsd2FsUHNUL3k1SW1wQkNsNHpDeHN4RCsxYlFNd2xqUjBVPSIsInB1YmxpY0tleSI6eyJjb250ZW50IjoiTFMwdExTMUNSVWRKVGlCRFJWSlVTVVpKUTBGVVJTMHRMUzB0Q2sxSlNVUjBWRU5EUVhwMVowRjNTVUpCWjBsVlJrbGpZa3R0Tm1sM1lrdFlhelZXV21oTU1FbEpkbmhMUldSM2QwTm5XVWxMYjFwSmVtb3dSVUYzVFhjS1RucEZWazFDVFVkQk1WVkZRMmhOVFdNeWJHNWpNMUoyWTIxVmRWcEhWakpOVWpSM1NFRlpSRlpSVVVSRmVGWjZZVmRrZW1SSE9YbGFVekZ3WW01U2JBcGpiVEZzV2tkc2FHUkhWWGRJYUdOT1RXcEplRTFVU1RCTlJFRjRUVlJGZVZkb1kwNU5ha2w0VFZSSk1FMUVRWGxOVkVWNVYycEJRVTFHYTNkRmQxbElDa3R2V2tsNmFqQkRRVkZaU1V0dldrbDZhakJFUVZGalJGRm5RVVZPUlRoaVUxQk1ZemhtVjFwc09ITTJiM2xaVkdwUVZqZE9VRkZvWm1ZNWNIZFFXVW9LZDJRNVRFWjVNbk5rZFhneFRXaGtLelpKVnpkUFoxZENUMWsxZVZsRVJISmlTWFZXUmxkU2VXUlpXU3REWlRSaFdUWlBRMEZzYjNkblowcFhUVUUwUndwQk1WVmtSSGRGUWk5M1VVVkJkMGxJWjBSQlZFSm5UbFpJVTFWRlJFUkJTMEpuWjNKQ1owVkdRbEZqUkVGNlFXUkNaMDVXU0ZFMFJVWm5VVlZVVkRWcENuTlZjakp5YVhWRVlub3pVbW92VEZZNVRrbEZRbE5KZDBoM1dVUldVakJxUWtKbmQwWnZRVlV6T1ZCd2VqRlphMFZhWWpWeFRtcHdTMFpYYVhocE5Ga0tXa1E0ZDJKUldVUldVakJTUVZGSUwwSkhUWGRaV1ZwbVlVaFNNR05JVFRaTWVUbHVZVmhTYjJSWFNYVlpNamwwVERKT2IxbFhiSFZhTTFab1kyMVJkQXBoVnpGb1dqSldla3d5YUd4aVIzaDJURmhrZG1OdGVHdE1lVFZ1WVZoU2IyUlhTWFprTWpsNVlUSmFjMkl6WkhwTU0wcHNZa2RXYUdNeVZYVmxWMFowQ21KRlFubGFWMXA2VERKb2JGbFhVbnBNTWpGb1lWYzBkMDlSV1V0TGQxbENRa0ZIUkhaNlFVSkJVVkZ5WVVoU01HTklUVFpNZVRrd1lqSjBiR0pwTldnS1dUTlNjR0l5TlhwTWJXUndaRWRvTVZsdVZucGFXRXBxWWpJMU1GcFhOVEJNYlU1MllsUkJWMEpuYjNKQ1owVkZRVmxQTDAxQlJVTkNRV2g2V1RKb2JBcGFTRlp6V2xSQk1rSm5iM0pDWjBWRlFWbFBMMDFCUlVSQ1EyaHBUWHBGTTA1dFRYbE9lbVJzVFhwRk1FOVVVbWhaVkdzeVRXcFpNazFxVVRST1YwbDRDazU2YkdsUFJHTXdXa1JWTkZsVVdYaE5RbmRIUTJselIwRlJVVUpuTnpoM1FWRlJSVVJyVG5sYVYwWXdXbE5DVTFwWGVHeFpXRTVzVFVOelIwTnBjMGNLUVZGUlFtYzNPSGRCVVZWRlNGZE9iMWxYYkhWYU0xWm9ZMjFSZEdGWE1XaGFNbFo2VERKb2JHSkhlSFpNV0dSMlkyMTRhMDFDTUVkRGFYTkhRVkZSUWdwbk56aDNRVkZaUlVRelNteGFiazEyWVVkV2FGcElUWFppVjBad1ltcERRbWxuV1V0TGQxbENRa0ZJVjJWUlNVVkJaMUk0UWtodlFXVkJRakpCVGpBNUNrMUhja2Q0ZUVWNVdYaHJaVWhLYkc1T2QwdHBVMncyTkROcWVYUXZOR1ZMWTI5QmRrdGxOazlCUVVGQ2FFdGlOVnBFTUVGQlFWRkVRVVZqZDFKUlNXY0tZWFZsU214RE5UVlRRVmh4YkVwbVdHZDNPVVpYVEM5b2NVRllTbWRqZFV0a2NrUlRieTlRUjJseU9FTkpVVVJ4YUc4MlExZDZTekJMU0dob1dWcDBlQXBwU0V0VVIzZERaVzVsYlhFNWRXSk5XREpOTDNaTVZFWXJha0ZMUW1kbmNXaHJhazlRVVZGRVFYZE9iMEZFUW14QmFrRlNRV3A1TlU5WE56UnFSbkZZQ21WMk9XTlBMMnhoZUUxdGNXOTBaSE5KTm5oaU1rZGxXbXBETVhCd2RVWjJibWhXTW1SeWEwSmpVRTF1ZFdkUFVtbHdORU5OVVVORldqSjNjbTByVEhFS2NVeFFaVUYzUVVwU1RuQlZWREYxYmtOcFJ6RkRkWEZYUVRoWVVYWXpjelZEWlRSd2RGTm9lbk5TYld4WVJsZHJTMWRqTlVWSmF6MEtMUzB0TFMxRlRrUWdRMFZTVkVsR1NVTkJWRVV0TFMwdExRbz0ifX19fQ==",
          "integratedTime": 1669248680,
          "logIndex": 7722031,
          "logID": "c0d23d6ad406973f9559f3ba2d1ca01f84147d8ffc5b8445c224f98b9591801d"
        }
      },
      "Issuer": "https://token.actions.githubusercontent.com",
      "Subject": "https://github.com/chainguard-images/hello-world/.github/workflows/release.yaml@refs/heads/main",
      "githubWorkflowName": "Create Release",
      "githubWorkflowRef": "refs/heads/main",
      "githubWorkflowRepository": "chainguard-images/hello-world",
      "githubWorkflowSha": "b3176c277e31494aa962662485b179b874d58a61",
      "githubWorkflowTrigger": "schedule",
      "run_attempt": "1",
      "run_id": "3536597993",
      "sha": "b3176c277e31494aa962662485b179b874d58a61"
    }
  }
]
```

You can verify that the image was built in Github Actions in this repository from the `Issuer` and `Subject` fields.
</details>

## Build

This image is built with [melange](https://github.com/chainguard-dev/melange) and [apko](https://github.com/chainguard-dev/apko).

