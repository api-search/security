---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: premierlacrosseleague.com
  spf: true
hosts:
- cert_expires: Oct 15 18:52:35 2026 GMT
  host: premierlacrosseleague.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 23:55:12 2026 GMT
  host: stats.premierlacrosseleague.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 02:18:02 2026 GMT
  host: shop.premierlacrosseleague.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Premier Lacrosse League Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Premier Lacrosse League, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Premier Lacrosse League
provider_slug: premier-lacrosse-league
slug: premier-lacrosse-league-domain-security
source_filename: premier-lacrosse-league-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: premierlacrosseleague.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 18:52:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: stats.premierlacrosseleague.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 23:55:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: shop.premierlacrosseleague.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 02:18:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: premierlacrosseleague.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/premier-lacrosse-league/refs/heads/main/security/premier-lacrosse-league-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Sports
- Lacrosse
- Professional Sports League
- Sports Statistics
- Media and Entertainment
- Ecommerce
- Agent Commerce
- GraphQL
- Fantasy Sports
---
