---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: yummly.com
  spf: true
hosts:
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: www.yummly.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- host: developer.yummly.com
  https: false
- host: api.yummly.com
  https: false
kind: domain-security
layout: security
method: probed
name: Yummly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yummly, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Yummly
provider_slug: yummly
slug: yummly-domain-security
source_filename: yummly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.yummly.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: null\n- host: developer.yummly.com\n  https: false\n- host: api.yummly.com\n  https: false\ndomains:\n- domain: yummly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yummly/refs/heads/main/security/yummly-domain-security.yml
summary_line: TLSv1.2
tags:
- Recipes
- Food
- Cooking
- Recipe Search
- Food Discovery
- Deprecated
- Historical
---
