---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kitfinch.com
  spf: true
hosts:
- cert_expires: Dec 23 18:36:01 2026 GMT
  host: kitfinch.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kitfinch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kitfinch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kitfinch
provider_slug: kitfinch-com
slug: kitfinch-com-domain-security
source_filename: kitfinch-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kitfinch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 18:36:01 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: kitfinch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/kitfinch-com/security/kitfinch-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Software
- Trade
- Tools
- Recommendations
- Pricing
---
