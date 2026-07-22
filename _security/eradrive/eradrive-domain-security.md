---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: eradrive.space
  spf: false
hosts:
- cert_expires: Oct 16 08:05:41 2026 GMT
  host: www.eradrive.space
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eradrive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EraDrive, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: EraDrive
provider_slug: eradrive
slug: eradrive-domain-security
source_filename: eradrive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eradrive.space\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 08:05:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: eradrive.space\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eradrive/refs/heads/main/security/eradrive-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Space
- Aerospace
- Satellite
- Autonomy
- Artificial Intelligence
- Edge Computing
- Defense
---
