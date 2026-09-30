---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bluewillow.com
  spf: true
hosts:
- cert_expires: Dec 12 20:40:42 2026 GMT
  host: bluewillow.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bluewillow Biologics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BlueWillow Biologics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: BlueWillow Biologics
provider_slug: bluewillow-biologics
slug: bluewillow-biologics-domain-security
source_filename: bluewillow-biologics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bluewillow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 20:40:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bluewillow.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluewillow-biologics/refs/heads/main/security/bluewillow-biologics-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Biotechnology
- Intranasal Vaccines
- Clinical Stage
- Nanotechnology
- Health
- Company
---
