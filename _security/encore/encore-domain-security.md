---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: encore.dev
  spf: true
hosts:
- cert_expires: Sep 12 22:32:38 2026 GMT
  host: encore.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Encore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Encore, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Encore
provider_slug: encore
slug: encore-domain-security
source_filename: encore-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: encore.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 22:32:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: encore.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/encore/refs/heads/main/security/encore-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Backend
- Cloud Native
- Frameworks
- Go
- Infrastructure Automation
- Microservices
- Open Source
- TypeScript
---
