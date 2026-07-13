---
api_specs:
- filename: predicthq-openapi.yml
  format: yaml
  label: PredictHQ API
  slug: predicthq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/predicthq/refs/heads/main/openapi/predicthq-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: predicthq.com
  spf: true
hosts:
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: www.predicthq.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: api.predicthq.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Predicthq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PredictHQ, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PredictHQ
provider_slug: predicthq
slug: predicthq-domain-security
source_filename: predicthq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.predicthq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: null\n- host: api.predicthq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: predicthq.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/predicthq/refs/heads/main/security/predicthq-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Demand Intelligence
- Events
- Forecasting
- Machine Learning
- Real-World Events
---
