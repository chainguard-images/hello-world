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
| `latest` | `sha256:5c99d8ed73711e9c33aeb592029fcb427c0595c0aa07edfd8165dbfb9a3b1206`<br/>[View entry in Rekor](https://rekor.tlog.dev/?hash=sha256:5c99d8ed73711e9c33aeb592029fcb427c0595c0aa07edfd8165dbfb9a3b1206) | `amd64` `arm64` `armv7` |



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
        "docker-manifest-digest": "sha256:5c99d8ed73711e9c33aeb592029fcb427c0595c0aa07edfd8165dbfb9a3b1206"
      },
      "type": "cosign container image signature"
    },
    "optional": {
      "1.3.6.1.4.1.57264.1.1": "https://token.actions.githubusercontent.com",
      "1.3.6.1.4.1.57264.1.2": "schedule",
      "1.3.6.1.4.1.57264.1.3": "4b9fd35731ffcc83790a9a949c2754092e0c499e",
      "1.3.6.1.4.1.57264.1.4": "Create Release",
      "1.3.6.1.4.1.57264.1.5": "chainguard-images/hello-world",
      "1.3.6.1.4.1.57264.1.6": "refs/heads/main",
      "Bundle": {
        "SignedEntryTimestamp": "MEUCIQCrB/yncqH54tVYN/pGYoDWe+sGLAyc1Zhxk8n+X+4gnQIgXmoqolz5OtkJFbbbVDqKEwQFR9Y813SSC8RPGv4NiMQ=",
        "Payload": {
          "body": "eyJhcGlWZXJzaW9uIjoiMC4wLjEiLCJraW5kIjoiaGFzaGVkcmVrb3JkIiwic3BlYyI6eyJkYXRhIjp7Imhhc2giOnsiYWxnb3JpdGhtIjoic2hhMjU2IiwidmFsdWUiOiI5MjYxYjRjMDg0Y2QwN2RiZDQ5MzY2MmI4MTVkY2U5ZGEzZTc1YWJlNjdhMmE5MDk1Y2QwMzZkZDhiZmI2YmMxIn19LCJzaWduYXR1cmUiOnsiY29udGVudCI6Ik1FUUNJSGpOeDV2MWFNMW5wUUhiVldESTYyYVlnQS9UbnBHcmhWTnNSbnNhWkZ2NUFpQlo2Zzk4S0g4TFR1cGFyOXlPcGJBOHNBU3dTNTNVUWlPRDYxaUQ2SzVWbmc9PSIsInB1YmxpY0tleSI6eyJjb250ZW50IjoiTFMwdExTMUNSVWRKVGlCRFJWSlVTVVpKUTBGVVJTMHRMUzB0Q2sxSlNVUjBWRU5EUVhwMVowRjNTVUpCWjBsVlFVNUtUSE5LYWpSTVdUSkVVM2RKWjAxQ1JFWlRlVzE1VTBoQmQwTm5XVWxMYjFwSmVtb3dSVUYzVFhjS1RucEZWazFDVFVkQk1WVkZRMmhOVFdNeWJHNWpNMUoyWTIxVmRWcEhWakpOVWpSM1NFRlpSRlpSVVVSRmVGWjZZVmRrZW1SSE9YbGFVekZ3WW01U2JBcGpiVEZzV2tkc2FHUkhWWGRJYUdOT1RXcEplRTFVU1RWTlJFRjRUVlJGTkZkb1kwNU5ha2w0VFZSSk5VMUVRWGxOVkVVMFYycEJRVTFHYTNkRmQxbElDa3R2V2tsNmFqQkRRVkZaU1V0dldrbDZhakJFUVZGalJGRm5RVVV6Wm1zelVsQmFVMG96VVdkYVdHOXhMM1JYUnpjeGRFOVRNbkZXWlcxbVkwRnFjRW9LYUc5Q05sQmlhMVpMWW5NdllqaGFZVkpzT0dSMFVHbHRiSEJUWVVKNlltMW5TRTFWYjA4MVZ6VTJRWEpYVTJnMk9UWlBRMEZzYjNkblowcFhUVUUwUndwQk1WVmtSSGRGUWk5M1VVVkJkMGxJWjBSQlZFSm5UbFpJVTFWRlJFUkJTMEpuWjNKQ1owVkdRbEZqUkVGNlFXUkNaMDVXU0ZFMFJVWm5VVlV5VlZWVkNqbG1hV294UkhZNVdqTmhjRWRDZUhsbE5qSk1jVWgzZDBoM1dVUldVakJxUWtKbmQwWnZRVlV6T1ZCd2VqRlphMFZhWWpWeFRtcHdTMFpYYVhocE5Ga0tXa1E0ZDJKUldVUldVakJTUVZGSUwwSkhUWGRaV1ZwbVlVaFNNR05JVFRaTWVUbHVZVmhTYjJSWFNYVlpNamwwVERKT2IxbFhiSFZhTTFab1kyMVJkQXBoVnpGb1dqSldla3d5YUd4aVIzaDJURmhrZG1OdGVHdE1lVFZ1WVZoU2IyUlhTWFprTWpsNVlUSmFjMkl6WkhwTU0wcHNZa2RXYUdNeVZYVmxWMFowQ21KRlFubGFWMXA2VERKb2JGbFhVbnBNTWpGb1lWYzBkMDlSV1V0TGQxbENRa0ZIUkhaNlFVSkJVVkZ5WVVoU01HTklUVFpNZVRrd1lqSjBiR0pwTldnS1dUTlNjR0l5TlhwTWJXUndaRWRvTVZsdVZucGFXRXBxWWpJMU1GcFhOVEJNYlU1MllsUkJWMEpuYjNKQ1owVkZRVmxQTDAxQlJVTkNRV2g2V1RKb2JBcGFTRlp6V2xSQk1rSm5iM0pDWjBWRlFWbFBMMDFCUlVSQ1EyY3dXV3BzYlZwRVRURk9lazE0V20xYWFsbDZaM3BPZW10M1dWUnNhRTlVVVRWWmVra3pDazVVVVhkUFZFcHNUVWROTUU5VWJHeE5RbmRIUTJselIwRlJVVUpuTnpoM1FWRlJSVVJyVG5sYVYwWXdXbE5DVTFwWGVHeFpXRTVzVFVOelIwTnBjMGNLUVZGUlFtYzNPSGRCVVZWRlNGZE9iMWxYYkhWYU0xWm9ZMjFSZEdGWE1XaGFNbFo2VERKb2JHSkhlSFpNV0dSMlkyMTRhMDFDTUVkRGFYTkhRVkZSUWdwbk56aDNRVkZaUlVRelNteGFiazEyWVVkV2FGcElUWFppVjBad1ltcERRbWxuV1V0TGQxbENRa0ZJVjJWUlNVVkJaMUk0UWtodlFXVkJRakpCVGpBNUNrMUhja2Q0ZUVWNVdYaHJaVWhLYkc1T2QwdHBVMncyTkROcWVYUXZOR1ZMWTI5QmRrdGxOazlCUVVGQ2FFMUROVko0ZDBGQlFWRkVRVVZqZDFKUlNXY0tSa3AzV0ZjMk9TOHJiMjFNVnpOcFIxVjNWMkpHUm1seVQzTkZlblJTTVdsSFFtOTFNM0pOU1ZWVk9FTkpVVVJaYzFSNllrMXRNVkpvZERNelYxWktUQXB6TjJ0SEt6UlJiamRyYVc4dmNVUXlhVTF4Tmtnck1XcHJla0ZMUW1kbmNXaHJhazlRVVZGRVFYZE9iMEZFUW14QmFrVkJkMFp0Wnk5b1RuWnFaU3R0Q2xreE5VTkRlamR0V0doNWQzWlNkV3hJYzBveU9FbHlRbFIzZVV4ME5qTnJZbHB4T1hVM1VYZGpRVlJXUW5SaVltSktlaXRCYWtKeFlubzFRWGcwWldvS1JqbE9kRmxXWTJGU2RsVTVka1J4VGxkeGVVRXpVMlZTZVRkRU0wMXhXakEyYW1wSkwzVlljQzh4Y0UxVVNETldLMU5MYWpKNGR6MEtMUzB0TFMxRlRrUWdRMFZTVkVsR1NVTkJWRVV0TFMwdExRbz0ifX19fQ==",
          "integratedTime": 1669680687,
          "logIndex": 8047879,
          "logID": "c0d23d6ad406973f9559f3ba2d1ca01f84147d8ffc5b8445c224f98b9591801d"
        }
      },
      "Issuer": "https://token.actions.githubusercontent.com",
      "Subject": "https://github.com/chainguard-images/hello-world/.github/workflows/release.yaml@refs/heads/main",
      "githubWorkflowName": "Create Release",
      "githubWorkflowRef": "refs/heads/main",
      "githubWorkflowRepository": "chainguard-images/hello-world",
      "githubWorkflowSha": "4b9fd35731ffcc83790a9a949c2754092e0c499e",
      "githubWorkflowTrigger": "schedule",
      "run_attempt": "1",
      "run_id": "3569746219",
      "sha": "4b9fd35731ffcc83790a9a949c2754092e0c499e"
    }
  }
]
```

You can verify that the image was built in Github Actions in this repository from the `Issuer` and `Subject` fields.
</details>

## Build

This image is built with [melange](https://github.com/chainguard-dev/melange) and [apko](https://github.com/chainguard-dev/apko).

