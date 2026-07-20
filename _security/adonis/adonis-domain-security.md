---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: adonis.io
  spf: true
hosts:
- cert_expires: Sep 21 13:15:28 2026 GMT
  host: adonis.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: api.adonis.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adonis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adonis, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Adonis
provider_slug: adonis
slug: adonis-domain-security
source_filename: adonis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adonis.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 13:15:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.adonis.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: adonis.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adonis/refs/heads/main/security/adonis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Revenue Cycle Management
- RCM
- Medical Billing
- Health IT
- Eligibility Verification
- Claims
- Payments
- Artificial Intelligence
- Automation
---
