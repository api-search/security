---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: axis.xyz
  spf: true
hosts:
- cert_expires: Oct  2 08:19:34 2026 GMT
  host: axis.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Axis 2 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Axis 2, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Axis 2
provider_slug: axis-2
slug: axis-2-domain-security
source_filename: axis-2-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: axis.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 08:19:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: axis.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axis-2/refs/heads/main/security/axis-2-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Regulatory Intelligence
- Compliance
- Corporate Affairs
- Government Relations
- Knowledge Base
- GRC
---
