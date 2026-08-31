---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vertafore.com
  spf: true
hosts:
- cert_expires: Aug 19 12:22:32 2026 GMT
  host: www.vertafore.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  3 23:59:59 2026 GMT
  host: developer.vertafore.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 23:59:59 2026 GMT
  host: api.vertafore.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vertafore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vertafore, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vertafore
provider_slug: vertafore
slug: vertafore-domain-security
source_filename: vertafore-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vertafore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 12:22:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: developer.vertafore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  3 23:59:59 2026 GMT\n  hsts: false\n- host: api.vertafore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: vertafore.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vertafore/refs/heads/main/security/vertafore-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- InsurTech
- Agency Management
- Property and Casualty
- AMS360
- Sagitta
- ImageRight
- Comparative Rating
- Partner Gated
---
