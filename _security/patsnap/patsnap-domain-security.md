---
api_specs:
- filename: patsnap-openapi-original.json
  format: json
  label: Patsnap Open Platform API
  slug: patsnap-open-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/patsnap/refs/heads/main/openapi/patsnap-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: patsnap.com
  spf: true
hosts:
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: patsnap.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: open.patsnap.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: connect.patsnap.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Patsnap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Patsnap, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Patsnap
provider_slug: patsnap
slug: patsnap-domain-security
source_filename: patsnap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: patsnap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: open.patsnap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: false\n- host: connect.patsnap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: patsnap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/patsnap/refs/heads/main/security/patsnap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Technology
- Patents
- Intellectual Property
- Innovation Intelligence
- Patent Search
- Life Sciences
- R&D
- Analytics
- Artificial Intelligence
---
