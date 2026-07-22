---
api_specs:
- filename: stellaconnect-requests-openapi-original.yml
  format: yaml
  label: Agent Connect Requests API
  slug: agent-connect-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stellaconnect/refs/heads/main/openapi/stellaconnect-requests-openapi-original.yml
- filename: stellaconnect-data-return-openapi-original.yml
  format: yaml
  label: Agent Connect Data Return API
  slug: agent-connect-data-return-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stellaconnect/refs/heads/main/openapi/stellaconnect-data-return-openapi-original.yml
- filename: stellaconnect-user-management-openapi-original.yml
  format: yaml
  label: Agent Connect User Management API
  slug: agent-connect-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stellaconnect/refs/heads/main/openapi/stellaconnect-user-management-openapi-original.yml
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
- SaaS
---
