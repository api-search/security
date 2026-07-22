---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sudowrite.com
  spf: true
hosts:
- cert_expires: Sep  9 13:09:20 2026 GMT
  host: sudowrite.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sudowrite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sudowrite, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sudowrite
provider_slug: sudowrite
slug: sudowrite-domain-security
source_filename: sudowrite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sudowrite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 13:09:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sudowrite.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sudowrite/refs/heads/main/security/sudowrite-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Writing
- Fiction
- Creative Writing
- Generative AI
- Content Generation
- Authoring
- Publishing
- Productivity
---
