---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: numero.ai
  spf: true
hosts:
- cert_expires: Aug 25 03:06:13 2026 GMT
  host: numero.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Numero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Numero, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Numero
provider_slug: numero
slug: numero-domain-security
source_filename: numero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: numero.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 03:06:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: numero.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/numero/refs/heads/main/security/numero-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise Saas
- Political Campaigns
- Fundraising
- Donor Management
- CRM
- Email
- Nonprofit Technology
---
