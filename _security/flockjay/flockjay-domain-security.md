---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: flockjay.com
  spf: true
hosts:
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: flockjay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: api.flockjay.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_note: 'Corrected by hand on 2026-08-14. probe-domain-security.py recorded null because the host root returns HTTP 404; the 404 response itself carries strict-transport-security: max-age=31536000; includeSubDomains, as does every 200 from /api/. Verified with curl -I https://api.flockjay.com/ and https://api.flockjay.com/api/.'
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flockjay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flockjay, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Flockjay
provider_slug: flockjay
slug: flockjay-domain-security
source_filename: flockjay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flockjay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.flockjay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_note: >-\n    Corrected by hand on 2026-08-14. probe-domain-security.py recorded null because\n    the host root returns HTTP 404; the 404 response itself carries\n    strict-transport-security: max-age=31536000; includeSubDomains, as does every\n    200 from /api/. Verified with curl -I https://api.flockjay.com/ and\n    https://api.flockjay.com/api/.\ndomains:\n- domain: flockjay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flockjay/refs/heads/main/security/flockjay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Sales Enablement
- Sales Training
- Learning Management
- Revenue Operations
- AI Coaching
- Content Management
- Software-as-a-Service
- MCP
- Agent Native
- Authentication
---
