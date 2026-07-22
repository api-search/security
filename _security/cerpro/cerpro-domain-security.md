---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cerpro.io
  spf: true
hosts:
- cert_expires: Sep  3 08:28:09 2026 GMT
  host: cerpro.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cerpro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CERPRO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CERPRO
provider_slug: cerpro
slug: cerpro-domain-security
source_filename: cerpro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cerpro.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 08:28:09 2026 GMT\n  hsts: false\ndomains:\n- domain: cerpro.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cerpro/refs/heads/main/security/cerpro-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Manufacturing
- Quality Assurance
- Artificial Intelligence
- Manufacturing Intelligence
- Document Extraction
- SaaS
- Germany
- Metalworking
- Inspection
---
