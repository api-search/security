---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: asherbio.com
  spf: true
hosts:
- cert_expires: Nov  8 11:26:02 2026 GMT
  host: asherbio.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Asherbio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Asherbio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Asherbio
provider_slug: asherbio
slug: asherbio-domain-security
source_filename: asherbio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: asherbio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 11:26:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: asherbio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asherbio/refs/heads/main/security/asherbio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Biopharma
- Immunotherapy
- Oncology
- Cis-targeted
- Biotechnology
---
