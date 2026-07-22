---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: instil.io
  spf: true
hosts:
- cert_expires: Oct 14 23:55:40 2026 GMT
  host: www.instil.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Instil Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Instil, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Instil
provider_slug: instil
slug: instil-domain-security
source_filename: instil-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.instil.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:55:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: instil.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instil/refs/heads/main/security/instil-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Saas
- Nonprofit
- CRM
- Fundraising
- Donor Management
- Philanthropy
- Revenue Intelligence
---
