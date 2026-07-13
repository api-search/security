---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: relayfi.com
  spf: true
hosts:
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: relayfi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Relay Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Relay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Relay
provider_slug: relay-financial
slug: relay-financial-domain-security
source_filename: relay-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: relayfi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: relayfi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/relay-financial/refs/heads/main/security/relay-financial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Business Banking
- Fintech
- SMB
- Cash Flow
- Bill Pay
---
