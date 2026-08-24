---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lassenpeak.com
  spf: true
hosts:
- cert_expires: Oct  2 18:45:57 2026 GMT
  host: www.lassenpeak.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lassen Peak Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lassen Peak, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lassen Peak
provider_slug: lassen-peak
slug: lassen-peak-domain-security
source_filename: lassen-peak-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lassenpeak.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 18:45:57 2026 GMT\n  hsts: false\ndomains:\n- domain: lassenpeak.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lassen-peak/refs/heads/main/security/lassen-peak-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Public Safety
- Law Enforcement
- Security
- Weapon Detection
- Imaging Radar
- Hardware
- Devices
- Cloud
- Government
---
