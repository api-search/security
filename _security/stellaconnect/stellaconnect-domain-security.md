---
api_specs:
- filename: stellaconnect-coaching-api-openapi.yml
  format: yaml
  label: Stella Connect (Medallia Agent Connect) Coaching API
  slug: stellaconnect-coaching-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stellaconnect/refs/heads/main/openapi/stellaconnect-coaching-api-openapi.yml
- filename: stellaconnect-data-api-openapi.yml
  format: yaml
  label: Stella Connect (Medallia Agent Connect) Data API
  slug: stellaconnect-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stellaconnect/refs/heads/main/openapi/stellaconnect-data-api-openapi.yml
- filename: stellaconnect-employees-api-openapi.yml
  format: yaml
  label: Stella Connect (Medallia Agent Connect) Employees API
  slug: stellaconnect-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stellaconnect/refs/heads/main/openapi/stellaconnect-employees-api-openapi.yml
- filename: stellaconnect-qa-api-openapi.yml
  format: yaml
  label: Stella Connect (Medallia Agent Connect) Qa API
  slug: stellaconnect-qa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stellaconnect/refs/heads/main/openapi/stellaconnect-qa-api-openapi.yml
- filename: stellaconnect-recoveries-api-openapi.yml
  format: yaml
  label: Stella Connect (Medallia Agent Connect) Recoveries API
  slug: stellaconnect-recoveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stellaconnect/refs/heads/main/openapi/stellaconnect-recoveries-api-openapi.yml
- filename: stellaconnect-requests-api-openapi.yml
  format: yaml
  label: Stella Connect (Medallia Agent Connect) Requests API
  slug: stellaconnect-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stellaconnect/refs/heads/main/openapi/stellaconnect-requests-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: false
  domain: stellaconnect.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: medallia.com
  spf: true
hosts:
- cert_expires: Oct 17 18:04:25 2026 GMT
  host: stellaconnect.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 23:59:59 2026 GMT
  host: docs.medallia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: api.stellaconnect.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stellaconnect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stella Connect (Medallia Agent Connect), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present.'
provider_name: Stella Connect (Medallia Agent Connect)
provider_slug: stellaconnect
slug: stellaconnect-domain-security
source_filename: stellaconnect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stellaconnect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 18:04:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.medallia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.stellaconnect.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: stellaconnect.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n- domain: medallia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stellaconnect/refs/heads/main/security/stellaconnect-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Customer Service
- Customer Feedback
- Quality Assurance
- Coaching
- Contact Centers
- Surveys
- Customer Experience
- Software-as-a-Service
---
