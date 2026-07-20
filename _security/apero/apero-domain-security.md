---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aperohealth.com
  spf: false
hosts:
- cert_expires: Sep 25 04:11:48 2026 GMT
  host: aperohealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apero, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Apero
provider_slug: apero
slug: apero-domain-security
source_filename: apero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aperohealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 04:11:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aperohealth.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apero/refs/heads/main/security/apero-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise Saas
- Healthcare
- Health Tech
- Revenue Cycle Management
- Medical Billing
- Practice Management
- Insurance
- Payments
- API
- Webhooks
---
