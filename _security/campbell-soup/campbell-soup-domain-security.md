---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: thecampbellscompany.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: campbellskitchen.com
  spf: true
hosts:
- cert_expires: Oct  1 01:01:50 2026 GMT
  host: www.thecampbellscompany.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: developer.campbellskitchen.com
  https: false
kind: domain-security
layout: security
method: probed
name: Campbell Soup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Campbell Soup, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Campbell Soup
provider_slug: campbell-soup
slug: campbell-soup-domain-security
source_filename: campbell-soup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thecampbellscompany.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 01:01:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.campbellskitchen.com\n  https: false\ndomains:\n- domain: thecampbellscompany.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: campbellskitchen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/campbell-soup/refs/heads/main/security/campbell-soup-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Food
- Consumer Packaged Goods
- Recipes
- Brands
- Fortune 500
---
