---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: energaia.com
  spf: true
hosts:
- cert_expires: Oct 16 17:46:21 2026 GMT
  host: energaia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Energaia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EnerGaia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: EnerGaia
provider_slug: energaia
slug: energaia-domain-security
source_filename: energaia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: energaia.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 16 17:46:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: energaia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/energaia/refs/heads/main/security/energaia-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Spirulina
- Microalgae
- Alternative Protein
- Food Ingredients
- Sustainability
- Biotechnology
- Food and Beverage
---
