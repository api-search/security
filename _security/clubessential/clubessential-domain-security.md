---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: clubessential.com
  spf: true
hosts:
- cert_expires: Oct 12 04:39:58 2026 GMT
  host: www.clubessential.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clubessential Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clubessential, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Clubessential
provider_slug: clubessential
slug: clubessential-domain-security
source_filename: clubessential-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clubessential.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 04:39:58 2026 GMT\n  hsts: null\ndomains:\n- domain: clubessential.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clubessential/refs/heads/main/security/clubessential-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Club Management
- Country Clubs
- Golf
- Hospitality
- SaaS
- Membership Management
- Point of Sale
- CRM
---
