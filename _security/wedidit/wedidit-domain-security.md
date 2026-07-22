---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: wedid.it
  spf: false
hosts:
- cert_expires: Oct 11 06:25:13 2026 GMT
  host: wedid.it
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wedidit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WeDidIt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: WeDidIt
provider_slug: wedidit
slug: wedidit-domain-security
source_filename: wedidit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wedid.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 06:25:13 2026 GMT\n  hsts: null\ndomains:\n- domain: wedid.it\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wedidit/refs/heads/main/security/wedidit-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Nonprofits
- Fundraising
- Crowdfunding
- Donations
- Acquired
---
