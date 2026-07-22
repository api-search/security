---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sensefinity.com
  spf: true
hosts:
- cert_expires: Oct 12 19:14:43 2026 GMT
  host: sensefinity.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sensefinity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sensefinity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Sensefinity
provider_slug: sensefinity
slug: sensefinity-domain-security
source_filename: sensefinity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sensefinity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 19:14:43 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: sensefinity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sensefinity/refs/heads/main/security/sensefinity-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Internet of Things
- Supply Chain
- Logistics
- Cold Chain
- Asset Tracking
- Sensors
- Cargo
---
