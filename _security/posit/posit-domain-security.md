---
api_specs:
- filename: posit-connect-openapi-original.json
  format: json
  label: Posit Connect Server API
  slug: posit-connect-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/posit/refs/heads/main/openapi/posit-connect-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: posit.co
  spf: true
hosts:
- cert_expires: Oct  7 23:59:59 2026 GMT
  host: posit.co
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: docs.posit.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Posit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Posit, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Posit
provider_slug: posit
slug: posit-domain-security
source_filename: posit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: posit.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: docs.posit.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: posit.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/posit/refs/heads/main/security/posit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Science
- Analytics
- Developer Tools
- R
- Python
- Publishing
- Machine Learning
- Enterprise
- Reproducibility
---
