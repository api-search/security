---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: lumafield.com
  spf: true
hosts:
- cert_expires: Oct 14 22:50:34 2026 GMT
  host: www.lumafield.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lumafield Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lumafield, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Lumafield
provider_slug: lumafield
slug: lumafield-domain-security
source_filename: lumafield-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lumafield.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 22:50:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lumafield.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lumafield/refs/heads/main/security/lumafield-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Manufacturing
- Industrial CT
- Inspection
- Hardware
- Analysis
- Quality
- Computer Vision
---
