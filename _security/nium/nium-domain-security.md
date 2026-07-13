---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nium.com
  spf: true
hosts:
- cert_expires: Aug 31 13:19:34 2026 GMT
  host: docs.nium.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 14 07:15:43 2027 GMT
  host: gateway.nium.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nium Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nium, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nium
provider_slug: nium
slug: nium-domain-security
source_filename: nium-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.nium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 13:19:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: gateway.nium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 07:15:43 2027 GMT\n  hsts: null\ndomains:\n- domain: nium.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nium/refs/heads/main/security/nium-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fintech
- Cross-Border
- Payments
- FX
- Issuing
---
