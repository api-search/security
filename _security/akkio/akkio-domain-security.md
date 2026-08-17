---
api_specs:
- filename: akkio-public-api-openapi.yaml
  format: yaml
  label: Akkio Public API (Beta)
  slug: akkio-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akkio/refs/heads/main/openapi/_original/akkio-public-api-openapi.yaml
- filename: akkio-datasets-api-openapi.yml
  format: yaml
  label: Akkio Datasets API
  slug: akkio-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akkio/refs/heads/main/openapi/akkio-datasets-api-openapi.yml
- filename: akkio-models-api-openapi.yml
  format: yaml
  label: Akkio Models API
  slug: akkio-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akkio/refs/heads/main/openapi/akkio-models-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "awstrust.com"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "pki.goog"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: akkio.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: akk.io
  spf: false
hosts:
- cert_expires: Oct 10 02:49:15 2026 GMT
  host: www.akkio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 05:48:40 2026 GMT
  host: docs.akkio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: api.akk.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Akkio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Akkio, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Akkio
provider_slug: akkio
slug: akkio-domain-security
source_filename: akkio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.akkio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 02:49:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.akkio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 05:48:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.akk.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: akkio.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: akk.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akkio/refs/heads/main/security/akkio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Apps
- Machine Learning
- Predictive Analytics
- No Code
- Data Science
- Marketing
- Media
- Audience Modeling
- Predictions
---
