---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: incredo.com
  spf: true
hosts:
- cert_expires: Sep 18 05:02:08 2026 GMT
  host: www.incredo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Douxmatok Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DouxMatok, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: DouxMatok
provider_slug: douxmatok
slug: douxmatok-domain-security
source_filename: douxmatok-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.incredo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 05:02:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: incredo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/douxmatok/refs/heads/main/security/douxmatok-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Food Technology
- Ingredients
- Sugar Reduction
- Manufacturing
- Consumer Packaged Goods
- Israel
---
