# sbom-util-SBOM-Attestation-Generator
A command-line tool that produces a signed attestation over a named SBOM and its digest, using DSSE. It takes an SBOM file and a private key as input, hashes the SBOM, hands the signer a payload that names the SBOM file as its subject with the digest under a named key, and writes the signed attestation document. This tool has no verify function. Verification is left to standard DSSE tooling. - Focused on Tools for generating and analyzing Software Bill of Materials (SBOMs) from Python packages and requirements files. This helps identify vulnerabilities and track dependencies across projects.

The run refuses at exit 1, before any write, when the output path resolves to the same file as the SBOM file or the private key file.

## Install
`git clone https://github.com/ShadowStrikeHQ/sbom-util-sbom-attestation-generator`
`pip install -r requirements.txt`

The install names `dsse`, the distribution that provides the `dsse` import used in the code.

## Usage
`./sbom-util-sbom-attestation-generator [params]`

## Parameters
- `-h`: Show help message and exit
- `--algorithm`: No description provided
- `--payload-type`: No description provided

## License
Copyright (c) ShadowStrikeHQ
