---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: belden.com
  spf: true
hosts:
- cert_expires: Aug 23 10:57:24 2026 GMT
  host: www.belden.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Belden Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Belden, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Belden
provider_slug: belden
slug: belden-domain-security
source_filename: belden-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.belden.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 10:57:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: belden.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/belden/refs/heads/main/security/belden-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Broadcast
- Cable
- Connectivity
- Industrial Automation
- Industrial Ethernet
- IIoT
- Networking
- Signal Transmission
- Smart Buildings
- Fortune 1000
---
