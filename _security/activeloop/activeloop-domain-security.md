---
api_specs:
- filename: activeloop-openapi.yml
  format: yaml
  label: Deep Lake SDK (Python)
  slug: deep-lake-python-sdk
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activeloop/refs/heads/main/openapi/activeloop-openapi.yml
- filename: activeloop-openapi.yml
  format: yaml
  label: Tensor Query Language (TQL)
  slug: tensor-query-language
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activeloop/refs/heads/main/openapi/activeloop-openapi.yml
- filename: activeloop-openapi.yml
  format: yaml
  label: Deep Lake Vector Store
  slug: vector-store
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activeloop/refs/heads/main/openapi/activeloop-openapi.yml
- filename: activeloop-openapi.yml
  format: yaml
  label: Activeloop Managed Database REST API
  slug: managed-database-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activeloop/refs/heads/main/openapi/activeloop-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: activeloop.ai
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: deeplake.ai
  spf: true
hosts:
- cert_expires: Oct  3 12:27:20 2026 GMT
  host: www.activeloop.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 08:31:50 2026 GMT
  host: docs.deeplake.ai
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 07:47:51 2026 GMT
  host: docs-v3.activeloop.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Activeloop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Activeloop, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Activeloop
provider_slug: activeloop
slug: activeloop-domain-security
source_filename: activeloop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.activeloop.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 12:27:20 2026 GMT\n  hsts: false\n- host: docs.deeplake.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 08:31:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: docs-v3.activeloop.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 07:47:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: activeloop.ai\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: deeplake.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/activeloop/refs/heads/main/security/activeloop-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Vector Store
- Data Lake
- Multimodal
- Deep Learning
- Python SDK
---
