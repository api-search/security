---
api_specs:
- filename: vanta-auditors-api-openapi.yml
  format: yaml
  label: Vanta Auditors API
  slug: vanta-auditors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vanta/refs/heads/main/openapi/vanta-auditors-api-openapi.yml
- filename: vanta-audits-api-openapi.yml
  format: yaml
  label: Vanta Audits API
  slug: vanta-audits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vanta/refs/heads/main/openapi/vanta-audits-api-openapi.yml
- filename: vanta-authentication-api-openapi.yml
  format: yaml
  label: Vanta Authentication API
  slug: vanta-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vanta/refs/heads/main/openapi/vanta-authentication-api-openapi.yml
- filename: vanta-controls-api-openapi.yml
  format: yaml
  label: Vanta Controls API
  slug: vanta-controls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vanta/refs/heads/main/openapi/vanta-controls-api-openapi.yml
- filename: vanta-documents-api-openapi.yml
  format: yaml
  label: Vanta Documents API
  slug: vanta-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vanta/refs/heads/main/openapi/vanta-documents-api-openapi.yml
- filename: vanta-integrations-api-openapi.yml
  format: yaml
  label: Vanta Integrations API
  slug: vanta-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vanta/refs/heads/main/openapi/vanta-integrations-api-openapi.yml
- filename: vanta-resources-api-openapi.yml
  format: yaml
  label: Vanta Resources API
  slug: vanta-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vanta/refs/heads/main/openapi/vanta-resources-api-openapi.yml
- filename: vanta-tests-api-openapi.yml
  format: yaml
  label: Vanta Tests API
  slug: vanta-tests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vanta/refs/heads/main/openapi/vanta-tests-api-openapi.yml
- filename: vanta-users-api-openapi.yml
  format: yaml
  label: Vanta Users API
  slug: vanta-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vanta/refs/heads/main/openapi/vanta-users-api-openapi.yml
- filename: vanta-vendors-api-openapi.yml
  format: yaml
  label: Vanta Vendors API
  slug: vanta-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vanta/refs/heads/main/openapi/vanta-vendors-api-openapi.yml
- filename: vanta-vulnerabilities-api-openapi.yml
  format: yaml
  label: Vanta Vulnerabilities API
  slug: vanta-vulnerabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vanta/refs/heads/main/openapi/vanta-vulnerabilities-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vanta.com
  spf: true
hosts:
- cert_expires: Aug 13 16:21:37 2026 GMT
  host: developer.vanta.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: api.vanta.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vanta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vanta, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Vanta
provider_slug: vanta
slug: vanta-domain-security
source_filename: vanta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.vanta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 16:21:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.vanta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: vanta.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vanta/refs/heads/main/security/vanta-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cybersecurity
- Compliance
- Security
- Governance
- Risk Management
---
