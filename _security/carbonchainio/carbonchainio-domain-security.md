---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: carbonchain.com
  spf: true
hosts:
- cert_expires: Dec 13 10:36:00 2026 GMT
  host: www.carbonchain.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Carbonchainio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carbonchainio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Carbonchainio
provider_slug: carbonchainio
slug: carbonchainio-domain-security
source_filename: carbonchainio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.carbonchain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 10:36:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: carbonchain.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carbonchainio/refs/heads/main/security/carbonchainio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Carbon Accounting
- Supply Chain
- Sustainability
- Emissions
- CBAM
---
