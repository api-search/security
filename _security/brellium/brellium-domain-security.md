---
api_specs:
- filename: brellium-audits-api-openapi.yml
  format: yaml
  label: Brellium Audits API
  slug: brellium-audits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brellium/refs/heads/main/openapi/brellium-audits-api-openapi.yml
- filename: brellium-auth-api-openapi.yml
  format: yaml
  label: Brellium Auth API
  slug: brellium-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brellium/refs/heads/main/openapi/brellium-auth-api-openapi.yml
- filename: brellium-coding-api-openapi.yml
  format: yaml
  label: Brellium Coding API
  slug: brellium-coding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brellium/refs/heads/main/openapi/brellium-coding-api-openapi.yml
- filename: brellium-documents-api-openapi.yml
  format: yaml
  label: Brellium Documents API
  slug: brellium-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brellium/refs/heads/main/openapi/brellium-documents-api-openapi.yml
- filename: brellium-documents-multiple-api-openapi.yml
  format: yaml
  label: Brellium Documents Multiple API
  slug: brellium-documents-multiple-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brellium/refs/heads/main/openapi/brellium-documents-multiple-api-openapi.yml
- filename: brellium-link-providers-api-openapi.yml
  format: yaml
  label: Brellium Link Providers API
  slug: brellium-link-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brellium/refs/heads/main/openapi/brellium-link-providers-api-openapi.yml
- filename: brellium-question-sets-api-openapi.yml
  format: yaml
  label: Brellium Question Sets API
  slug: brellium-question-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brellium/refs/heads/main/openapi/brellium-question-sets-api-openapi.yml
- filename: brellium-update-audits-flags-api-openapi.yml
  format: yaml
  label: Brellium Update Audits Flags API
  slug: brellium-update-audits-flags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brellium/refs/heads/main/openapi/brellium-update-audits-flags-api-openapi.yml
- filename: brellium-users-api-openapi.yml
  format: yaml
  label: Brellium Users API
  slug: brellium-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brellium/refs/heads/main/openapi/brellium-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: brellium.com
  spf: true
hosts:
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: api.brellium.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brellium Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brellium, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Brellium
provider_slug: brellium
slug: brellium-domain-security
source_filename: brellium-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.brellium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: brellium.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brellium/refs/heads/main/security/brellium-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Clinical Compliance
- Clinical Documentation
- Medical Coding
- Audit
- Behavioral Health
- Digital Health
- API
---
