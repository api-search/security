---
api_specs:
- filename: definedcrowd-openapi-original.json
  format: json
  label: Defined.ai Public API
  slug: definedai-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/definedcrowd/refs/heads/main/openapi/definedcrowd-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: definedcrowd.com
  spf: true
hosts:
- cert_expires: Sep  6 15:38:14 2026 GMT
  host: www.definedcrowd.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 15:38:14 2026 GMT
  host: developers.definedcrowd.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 15:38:14 2026 GMT
  host: api.production-na01.definedcrowd.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Definedcrowd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Defined.ai (DefinedCrowd), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Defined.ai (DefinedCrowd)
provider_slug: definedcrowd
slug: definedcrowd-domain-security
source_filename: definedcrowd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.definedcrowd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 15:38:14 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developers.definedcrowd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 15:38:14 2026 GMT\n  hsts: false\n- host: api.production-na01.definedcrowd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 15:38:14 2026 GMT\n  hsts: null\ndomains:\n- domain: definedcrowd.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/definedcrowd/refs/heads/main/security/definedcrowd-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Training Data
- Data Marketplace
- Machine Learning
- Data Annotation
- Speech Data
- Natural Language Processing
- Crowdsourcing
- Artificial Intelligence
---
