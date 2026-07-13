---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gem.com
  spf: true
hosts:
- cert_expires: Oct  3 00:03:10 2026 GMT
  host: www.gem.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: api.gem.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 23:09:45 2026 GMT
  host: app.gem.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gem Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gem, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gem
provider_slug: gem-com
slug: gem-com-domain-security
source_filename: gem-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gem.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 00:03:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.gem.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: null\n- host: app.gem.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:09:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: gem.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gem-com/refs/heads/main/security/gem-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Recruiting CRM
- ATS
- Sourcing
- Talent Marketing
- Agentic AI
- HR Tech
---
