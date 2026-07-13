---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: campbells.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: campbellskitchen.com
  spf: true
hosts:
- cert_expires: Sep 14 08:26:15 2026 GMT
  host: www.campbells.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: developer.campbellskitchen.com
  https: false
kind: domain-security
layout: security
method: probed
name: Campbells Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Campbell''s, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Campbell's
provider_slug: campbells
slug: campbells-domain-security
source_filename: campbells-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.campbells.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:26:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.campbellskitchen.com\n  https: false\ndomains:\n- domain: campbells.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: campbellskitchen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/campbells/refs/heads/main/security/campbells-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Food
- Consumer Packaged Goods
- Recipes
- Brands
---
