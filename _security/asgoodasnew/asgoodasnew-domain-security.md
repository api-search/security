---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: asgoodasnew.com
  spf: true
hosts:
- cert_expires: Mar 13 23:59:59 2027 GMT
  host: asgoodasnew.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Asgoodasnew Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for asgoodasnew, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: asgoodasnew
provider_slug: asgoodasnew
slug: asgoodasnew-domain-security
source_filename: asgoodasnew-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: asgoodasnew.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 13 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: asgoodasnew.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asgoodasnew/refs/heads/main/security/asgoodasnew-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ecommerce
- Retail
- Refurbished Electronics
- Consumer Electronics
- Germany
---
