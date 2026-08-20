---
api_specs:
- filename: shieldlabs-server-api-openapi.yml
  format: yaml
  label: ShieldLabs Server API
  slug: shieldlabs-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shieldlabs/refs/heads/main/openapi/shieldlabs-server-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: shieldlabs.ai
  spf: true
hosts:
- cert_expires: Oct 11 21:20:55 2026 GMT
  host: docs.shieldlabs.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 06:19:00 2026 GMT
  host: api.shieldlabs.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 16:49:57 2026 GMT
  host: account.shieldlabs.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shieldlabs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ShieldLabs, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ShieldLabs
provider_slug: shieldlabs
slug: shieldlabs-domain-security
source_filename: shieldlabs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.shieldlabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 21:20:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.shieldlabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 06:19:00 2026 GMT\n  hsts: null\n- host: account.shieldlabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 16:49:57 2026 GMT\n  hsts: null\ndomains:\n- domain: shieldlabs.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shieldlabs/refs/heads/main/security/shieldlabs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fraud Detection
- Abuse Prevention
- Visitor Identification
- Device Fingerprinting
- Bot Detection
- vpn-proxy-detection
- Risk Scoring
- Identity
- Security
- Webhook
- Anti-Fraud
- traffic-quality
---
