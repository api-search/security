---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: iflowinc.com
  spf: true
hosts:
- cert_expires: Aug 16 15:48:00 2026 GMT
  host: iflowinc.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: I Flow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for I Flow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: I Flow
provider_slug: i-flow
slug: i-flow-domain-security
source_filename: i-flow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iflowinc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 15:48:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: iflowinc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/i-flow/refs/heads/main/security/i-flow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Water
- Metering
- Sustainability
- IoT
---
