---
api_specs:
- filename: zylo-enterprise-openapi.yml
  format: yaml
  label: Zylo Enterprise API
  slug: enterprise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zylo/refs/heads/main/openapi/zylo-enterprise-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zylo.com
  spf: true
hosts:
- cert_expires: Oct  1 02:30:41 2026 GMT
  host: zylo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 21:26:49 2026 GMT
  host: developer.zylo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: api.zylo.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Zylo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zylo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zylo
provider_slug: zylo
slug: zylo-domain-security
source_filename: zylo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zylo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 02:30:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.zylo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 21:26:49 2026 GMT\n  hsts: null\n- host: api.zylo.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: zylo.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zylo/refs/heads/main/security/zylo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Budgets
- SaaS Management
- Spend
---
