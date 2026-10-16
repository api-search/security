---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: biogaia.com
  spf: true
hosts:
- cert_expires: Nov 16 17:55:32 2026 GMT
  host: www.biogaia.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Biogaia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BioGaia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BioGaia
provider_slug: biogaia
slug: biogaia-domain-security
source_filename: biogaia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.biogaia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 17:55:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: biogaia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biogaia/refs/heads/main/security/biogaia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Probiotics
- Healthcare
- Sweden
- GutHealth
- ConsumerProducts
---
