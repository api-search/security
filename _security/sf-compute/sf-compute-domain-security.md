---
api_specs:
- filename: sf-compute-openapi.yml
  format: yaml
  label: SF Compute Orders API
  slug: orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sf-compute/refs/heads/main/openapi/sf-compute-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sfcompute.com
  spf: true
hosts:
- cert_expires: Aug 26 04:20:16 2026 GMT
  host: sfcompute.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 04:20:16 2026 GMT
  host: docs.sfcompute.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: api.sfcompute.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Sf Compute Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for San Francisco Compute Company, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: San Francisco Compute Company
provider_slug: sf-compute
slug: sf-compute-domain-security
source_filename: sf-compute-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sfcompute.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 04:20:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.sfcompute.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 04:20:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.sfcompute.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: sfcompute.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sf-compute/refs/heads/main/security/sf-compute-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Cloud
- Clusters
- Compute
- GPU
- Machine Learning
- Marketplace
- Training
---
