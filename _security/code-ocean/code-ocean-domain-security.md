---
api_specs:
- filename: code-ocean-openapi.yml
  format: yaml
  label: Code Ocean API
  slug: code-ocean-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/code-ocean/refs/heads/main/openapi/code-ocean-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue ";"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: codeocean.com
  spf: true
hosts:
- cert_expires: Aug 31 13:44:49 2026 GMT
  host: docs.codeocean.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  3 23:59:59 2027 GMT
  host: codeocean.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Code Ocean Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Code Ocean, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Code Ocean
provider_slug: code-ocean
slug: code-ocean-domain-security
source_filename: code-ocean-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.codeocean.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 13:44:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: codeocean.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: codeocean.com\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \";\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/code-ocean/refs/heads/main/security/code-ocean-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Reproducible Research
- Computational Science
- Data Science
- Research Computing
- Life Sciences
- Pipelines
- MLOps
- Cloud Platform
- Developer Tools
---
