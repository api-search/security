---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: alwayz.co
  spf: false
hosts:
- cert_expires: Aug 19 10:27:46 2026 GMT
  host: alwayz.co
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Levit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Levit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Levit
provider_slug: levit
slug: levit-domain-security
source_filename: levit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alwayz.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 19 10:27:46 2026 GMT\n  hsts: false\ndomains:\n- domain: alwayz.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/levit/refs/heads/main/security/levit-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Commerce
- E-commerce
- Marketplace
- Retail
- Mobile
- Group Buying
- Consumer
- South Korea
---
