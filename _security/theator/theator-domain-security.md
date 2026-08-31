---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "digicert.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: theator.io
  spf: true
hosts:
- cert_expires: Oct 17 09:41:29 2026 GMT
  host: theator.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Theator Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Theator, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Theator
provider_slug: theator
slug: theator-domain-security
source_filename: theator-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: theator.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 09:41:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: theator.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/theator/refs/heads/main/security/theator-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Surgery
- Surgical Intelligence
- Medical Video
- Artificial Intelligence
- Clinical Analytics
- HealthTech
---
