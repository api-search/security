---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zimmerbiomet.com
  spf: true
hosts:
- cert_expires: Oct  4 18:36:18 2026 GMT
  host: www.zimmerbiomet.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zimmer Biomet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zimmer Biomet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zimmer Biomet
provider_slug: zimmer-biomet
slug: zimmer-biomet-domain-security
source_filename: zimmer-biomet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zimmerbiomet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 18:36:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: zimmerbiomet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zimmer-biomet/refs/heads/main/security/zimmer-biomet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Medical Devices
- Orthopedics
- Healthcare
- Robotics
- Fortune 500
---
