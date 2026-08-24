---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: goodmeat.co
  spf: true
hosts:
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: www.goodmeat.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Good Meat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GOOD Meat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GOOD Meat
provider_slug: good-meat
slug: good-meat-domain-security
source_filename: good-meat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.goodmeat.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: goodmeat.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/good-meat/refs/heads/main/security/good-meat-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Food and Beverage
- Cultivated Meat
- Agriculture Technology
- Consumer Packaged Goods
- Biotechnology
- Food Technology
- Sustainability
---
