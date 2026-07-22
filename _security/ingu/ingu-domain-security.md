---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ingu.com
  spf: true
hosts:
- cert_expires: Oct  9 08:33:30 2026 GMT
  host: ingu.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ingu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for INGU, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: INGU
provider_slug: ingu
slug: ingu-domain-security
source_filename: ingu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ingu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 08:33:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ingu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ingu/refs/heads/main/security/ingu-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Pipeline Integrity
- Inline Inspection
- Oil and Gas
- Water and Wastewater
- Leak Detection
- Industrial IoT
- GIS
---
