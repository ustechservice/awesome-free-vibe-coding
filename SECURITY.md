# Security Policy

This repository is a documentation project — it ships no executable code beyond CI workflows. Security concerns here mean:

## Reporting

- **Malicious links or compromised tools listed in the directory**: open an issue with the `security` label, or use GitHub's private vulnerability reporting on this repo if disclosure timing matters.
- **CI workflow concerns**: same channel.

We treat "a listed tool turned malicious or was compromised" as a security report, not a stale-data report — it gets priority handling and immediate removal pending investigation.

## Scope

In scope: directory content that could route users to harm (typosquatted links, compromised projects, tools discovered to exfiltrate code or credentials beyond their disclosed behavior).
Out of scope: vulnerabilities in the listed tools themselves — report those upstream to the tool's own security process. We will, however, add a ⚠️ advisory note with a source link for significant public incidents.
