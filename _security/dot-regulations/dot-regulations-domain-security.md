---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: transportation.gov
  spf: true
hosts:
- cert_expires: Jul 21 23:59:59 2026 GMT
  host: www.transportation.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dot Regulations Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DOT Regulations, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: DOT Regulations
provider_slug: dot-regulations
slug: dot-regulations-domain-security
source_filename: dot-regulations-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.transportation.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: transportation.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dot-regulations/refs/heads/main/security/dot-regulations-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Compliance
- Federal Government
- Regulations
- Safety
- Transportation
---
