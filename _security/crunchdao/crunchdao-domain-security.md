---
api_specs:
- filename: crunchdao-tournament-openapi.json
  format: json
  label: CrunchDAO Tournament API
  slug: crunchdao-tournament-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crunchdao/refs/heads/main/openapi/crunchdao-tournament-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: crunchdao.com
  spf: true
hosts:
- cert_expires: Sep 29 09:57:37 2026 GMT
  host: crunchdao.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 23:03:49 2026 GMT
  host: api.hub.crunchdao.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crunchdao Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CrunchDAO, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: CrunchDAO
provider_slug: crunchdao
slug: crunchdao-domain-security
source_filename: crunchdao-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crunchdao.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 09:57:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.hub.crunchdao.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 23:03:49 2026 GMT\n  hsts: false\ndomains:\n- domain: crunchdao.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crunchdao/refs/heads/main/security/crunchdao-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto Web3
- Machine Learning
- Data Science
- Competitions
- Collective Intelligence
- Quantitative Finance
- Predictions
---
