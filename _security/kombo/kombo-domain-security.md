---
api_specs:
- filename: kombo-ai-apply-api-openapi.yml
  format: yaml
  label: Kombo AI Apply API
  slug: kombo-ai-apply-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kombo/refs/heads/main/openapi/kombo-ai-apply-api-openapi.yml
- filename: kombo-custom-endpoints-api-openapi.yml
  format: yaml
  label: Kombo Custom Endpoints API
  slug: kombo-custom-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kombo/refs/heads/main/openapi/kombo-custom-endpoints-api-openapi.yml
- filename: kombo-general-api-openapi.yml
  format: yaml
  label: Kombo General API
  slug: kombo-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kombo/refs/heads/main/openapi/kombo-general-api-openapi.yml
- filename: kombo-kombo-connect-api-openapi.yml
  format: yaml
  label: Kombo Kombo Connect API
  slug: kombo-kombo-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kombo/refs/heads/main/openapi/kombo-kombo-connect-api-openapi.yml
- filename: kombo-unified-ats-api-api-openapi.yml
  format: yaml
  label: Kombo Unified ATS API API
  slug: kombo-unified-ats-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kombo/refs/heads/main/openapi/kombo-unified-ats-api-api-openapi.yml
- filename: kombo-unified-ats-assessment-background-check-api-api-openapi.yml
  format: yaml
  label: Kombo Unified ATS (Assessment & Background Check) API API
  slug: kombo-unified-ats-assessment-background-check-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kombo/refs/heads/main/openapi/kombo-unified-ats-assessment-background-check-api-api-openapi.yml
- filename: kombo-unified-hris-api-api-openapi.yml
  format: yaml
  label: Kombo Unified HRIS API API
  slug: kombo-unified-hris-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kombo/refs/heads/main/openapi/kombo-unified-hris-api-api-openapi.yml
- filename: kombo-unified-lms-api-api-openapi.yml
  format: yaml
  label: Kombo Unified LMS API API
  slug: kombo-unified-lms-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kombo/refs/heads/main/openapi/kombo-unified-lms-api-api-openapi.yml
- filename: kombo-kombo-api-api-openapi.yml
  format: yaml
  label: Kombo Kombo API
  slug: kombo-kombo-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kombo/refs/heads/main/openapi/kombo-kombo-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kombo.dev
  spf: true
hosts:
- cert_expires: Sep 11 05:13:52 2026 GMT
  host: www.kombo.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 11:07:52 2026 GMT
  host: api.kombo.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 08:26:49 2026 GMT
  host: docs.kombo.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kombo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kombo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kombo
provider_slug: kombo
slug: kombo-domain-security
source_filename: kombo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kombo.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 05:13:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.kombo.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 11:07:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.kombo.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 08:26:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: kombo.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kombo/refs/heads/main/security/kombo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- ATS
- Embedded iPaaS
- HRIS
- LMS
- Payroll
- Unified-API
---
