---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: humanitru.com
  spf: false
hosts:
- cert_expires: Aug 20 19:03:50 2026 GMT
  host: humanitru.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Humanitru Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Humanitru, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Humanitru
provider_slug: humanitru
slug: humanitru-domain-security
source_filename: humanitru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: humanitru.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 19:03:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: humanitru.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/humanitru/refs/heads/main/security/humanitru-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- CRM
- Nonprofit
- Fundraising
- Donor Management
- Integrations
- Membership
- Museums
---
