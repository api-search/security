---
api_specs:
- filename: figure-eight-openapi-original.json
  format: json
  label: Figure Eight API (Appen Platform API)
  slug: figure-eight-api-appen-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-eight/refs/heads/main/openapi/figure-eight-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: swaggerhub.com
  spf: true
- caa:
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.appen.com"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: appen.com
  spf: true
hosts:
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: app.swaggerhub.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: api.appen.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Figure Eight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Figure Eight, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Figure Eight
provider_slug: figure-eight
slug: figure-eight-domain-security
source_filename: figure-eight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: app.swaggerhub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: null\n- host: api.appen.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: swaggerhub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: appen.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.appen.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/figure-eight/refs/heads/main/security/figure-eight-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai
- Machine Learning
- Data Labeling
- Data Annotation
- Training Data
- Human-in-the-Loop
- Crowdsourcing
- Acquired
---
