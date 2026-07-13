---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: kinaxis.com
  spf: true
hosts:
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: www.kinaxis.com
  hsts: true
  hsts_max_age: 1000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 11:15:50 2026 GMT
  host: knowledge.kinaxis.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: rapidresponse.kinaxis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Kinaxis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kinaxis, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Kinaxis
provider_slug: kinaxis
slug: kinaxis-domain-security
source_filename: kinaxis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kinaxis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 1000\n- host: knowledge.kinaxis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 11:15:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: rapidresponse.kinaxis.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kinaxis.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kinaxis/refs/heads/main/security/kinaxis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Supply Chain
- Supply Chain Planning
- Demand Sensing
- Scenario Modeling
- Supply Planning
- Inventory Optimization
- S&OP
- Control Tower
- Enterprise Software
- AI
---
