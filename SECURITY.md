# Security Policy

## Supported Versions

Distroless currently tracks debian 12 ([bookworm](https://packages.debian.org/bookworm)) packages.

Debian package versions used for the current build are found in https://github.com/GoogleContainerTools/distroless/blob/main/private/repos/deb. It can be parsed and printed into simple json data by invoking `./knife deb-versions` at the root of this project.

## Reporting a Vulnerability

If a distroless image you are using contains a CVE or other vulnerability:
1. ensure you are using a [currently supported image](https://github.com/GoogleContainerTools/distroless#what-images-are-available)
1. find the appropriate debian security-tracker notice: `https://security-tracker.debian.org/tracker/CVE-XXXX-YYYYY`, for [example](https://security-tracker.debian.org/tracker/CVE-2022-21476).
1. check if a fix is available for the appropriate debian version in the main/security channels (ex `bookworm`, `bookworm (security)`).
    1. if a fix is not yet available, do not file a bug, track it in your internal tracker until one becomes available.
    1. if a fix is available *and* it has been more than 48 hours, please let the team know by creating an issue and pointing to the CVE or vulnerability disclosure.
