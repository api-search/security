---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: githubstatus.com
  spf: true
hosts:
- cert_expires: Jan 22 23:23:04 2027 GMT
  host: www.githubstatus.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GitHub CLI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GitHub CLI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: GitHub CLI
provider_slug: github-cli
slug: github-cli-domain-security
source_filename: github-cli-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.githubstatus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:23:04 2027 GMT\n  hsts: true\n  hsts_max_age: 259200\ndomains:\n- domain: githubstatus.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/github-cli/security/github-cli-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Command Line Interface
- Platform CLI
- Developer Tools
- Version Control
- Open Source
- GitHub
---
