---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: denalitherapeutics.com
  spf: false
hosts:
- cert_expires: Oct 12 14:31:22 2026 GMT
  host: denalitherapeutics.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Denali Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Denali Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Denali Therapeutics
provider_slug: denali-therapeutics
slug: denali-therapeutics-domain-security
source_filename: denali-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: denalitherapeutics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 14:31:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: denalitherapeutics.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/denali-therapeutics/refs/heads/main/security/denali-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Life Sciences
- Biotechnology
- Pharmaceuticals
- Neuroscience
- Neurodegenerative Diseases
- Drug Development
- Healthcare
---
