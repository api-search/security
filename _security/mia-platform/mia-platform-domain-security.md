---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mia-platform.eu
  spf: true
hosts:
- cert_expires: Oct  4 08:57:28 2026 GMT
  host: mia-platform.eu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mia Platform Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mia-Platform, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mia-Platform
provider_slug: mia-platform
slug: mia-platform-domain-security
source_filename: mia-platform-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mia-platform.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 08:57:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mia-platform.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mia-platform/refs/heads/main/security/mia-platform-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Native
- Developer Platform
- DevOps
- IDP
- Microservices
---
