---
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: palettehq.com
  spf: true
hosts:
- cert_expires: Sep 11 19:54:54 2026 GMT
  host: palettehq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Palette Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Palette, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Palette
provider_slug: palette
slug: palette-domain-security
source_filename: palette-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: palettehq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 19:54:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: palettehq.com\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/palette/refs/heads/main/security/palette-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Apps
- Sales Compensation
- Commission Management
- Revenue Operations
- Sales
- FinOps
- SaaS
---
