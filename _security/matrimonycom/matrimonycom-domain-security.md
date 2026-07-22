---
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issuewild "globalsign.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: matrimony.com
  spf: true
hosts:
- cert_expires: Apr 10 08:16:34 2027 GMT
  host: www.matrimony.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Matrimonycom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Matrimony.com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Matrimony.com
provider_slug: matrimonycom
slug: matrimonycom-domain-security
source_filename: matrimonycom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.matrimony.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 10 08:16:34 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: matrimony.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issuewild \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/matrimonycom/refs/heads/main/security/matrimonycom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Matchmaking
- Matrimony
- Weddings
- Marketplace
- India
---
