---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lollipuff.com
  spf: true
hosts:
- cert_expires: Aug 25 11:04:53 2026 GMT
  host: www.lollipuff.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lollipuff Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lollipuff, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lollipuff
provider_slug: lollipuff
slug: lollipuff-domain-security
source_filename: lollipuff-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lollipuff.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 11:04:53 2026 GMT\n  hsts: false\ndomains:\n- domain: lollipuff.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lollipuff/refs/heads/main/security/lollipuff-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Authentication
- Luxury Goods
- Designer Fashion
- Resale
- Marketplace
- Ecommerce
- Y Combinator
---
