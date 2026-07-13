---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: apiwiz.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: treblle.com
  spf: true
hosts:
- cert_expires: Aug 28 20:57:52 2026 GMT
  host: www.apiwiz.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 02:14:05 2026 GMT
  host: treblle.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 23:38:08 2026 GMT
  host: 42crunch.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Governance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for API Governance, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: API Governance
provider_slug: governance
slug: governance-domain-security
source_filename: governance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apiwiz.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 20:57:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: treblle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 02:14:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: 42crunch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:38:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: apiwiz.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: treblle.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/governance/refs/heads/main/security/governance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Governance
- Policies
- Rules
- Spectral
- Linting
- Lifecycle
- Compliance
- Standards
- OpenAPI
- AsyncAPI
---
