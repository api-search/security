---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: proton.me
  spf: true
hosts:
- cert_expires: Dec  1 13:13:51 2026 GMT
  host: proton.me
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Proton Me Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Proton Drive, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Proton Drive
provider_slug: proton-me
slug: proton-me-domain-security
source_filename: proton-me-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: proton.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 13:13:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: proton.me\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/proton-me/security/proton-me-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cloud Storage
- Privacy
- Encryption
- File Sharing
- Secure Collaboration
---
