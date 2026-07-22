---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: navabi.ca
  spf: false
hosts:
- cert_expires: Sep  1 04:40:54 2026 GMT
  host: www.navabi.ca
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Navabi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for navabi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: navabi
provider_slug: navabi
slug: navabi-domain-security
source_filename: navabi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.navabi.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 04:40:54 2026 GMT\n  hsts: false\ndomains:\n- domain: navabi.ca\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/navabi/refs/heads/main/security/navabi-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Retail
- Fashion
- E-commerce
- Apparel
- Plus Size Fashion
---
