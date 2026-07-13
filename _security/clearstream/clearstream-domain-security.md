---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: clearstream.com
  spf: true
hosts:
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: www.clearstream.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clearstream Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clearstream, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Clearstream
provider_slug: clearstream
slug: clearstream-domain-security
source_filename: clearstream-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clearstream.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: clearstream.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clearstream/refs/heads/main/security/clearstream-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Capital Markets
- Collateral Management
- Custody
- Financial Services
- ISO 15022
- ISO 20022
- Post-Trade Infrastructure
- Securities
- Settlement
- SWIFT
---
