---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: infarm.com
  spf: true
hosts:
- cert_expires: Sep 25 14:47:59 2026 GMT
  host: infarm.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Infarm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for infarm, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: infarm
provider_slug: infarm
slug: infarm-domain-security
source_filename: infarm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: infarm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 14:47:59 2026 GMT\n  hsts: null\ndomains:\n- domain: infarm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infarm/refs/heads/main/security/infarm-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Vertical Farming
- Agriculture
- AgTech
- Food
- Sustainability
---
