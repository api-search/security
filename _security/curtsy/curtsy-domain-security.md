---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: curtsyapp.com
  spf: true
hosts:
- cert_expires: Sep 24 10:01:26 2026 GMT
  host: curtsyapp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Curtsy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Curtsy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Curtsy
provider_slug: curtsy
slug: curtsy-domain-security
source_filename: curtsy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: curtsyapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 10:01:26 2026 GMT\n  hsts: null\ndomains:\n- domain: curtsyapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curtsy/refs/heads/main/security/curtsy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Resale
- Marketplace
- Fashion
- E-commerce
- Secondhand
- Consumer
- Mobile
---
