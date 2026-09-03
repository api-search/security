---
api_specs:
- filename: cadasto-ehr-api-openapi.json
  format: json
  label: Cadasto EHR API
  slug: cadasto-ehr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadasto/refs/heads/main/openapi/cadasto-ehr-api-openapi.json
- filename: cadasto-query-api-openapi.json
  format: json
  label: Cadasto Query API (AQL)
  slug: cadasto-query-api-aql
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadasto/refs/heads/main/openapi/cadasto-query-api-openapi.json
- filename: cadasto-definition-api-openapi.json
  format: json
  label: Cadasto Definition API
  slug: cadasto-definition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadasto/refs/heads/main/openapi/cadasto-definition-api-openapi.json
- filename: cadasto-demographic-api-openapi.json
  format: json
  label: Cadasto Demographic API
  slug: cadasto-demographic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadasto/refs/heads/main/openapi/cadasto-demographic-api-openapi.json
- filename: cadasto-admin-api-openapi.json
  format: json
  label: Cadasto Admin API
  slug: cadasto-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadasto/refs/heads/main/openapi/cadasto-admin-api-openapi.json
- filename: cadasto-system-api-openapi.json
  format: json
  label: Cadasto System API
  slug: cadasto-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadasto/refs/heads/main/openapi/cadasto-system-api-openapi.json
- filename: cadasto-extra-api-openapi.json
  format: json
  label: Cadasto Additional API
  slug: cadasto-additional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadasto/refs/heads/main/openapi/cadasto-extra-api-openapi.json
- filename: cadasto-smart-on-openehr-openapi.json
  format: json
  label: Cadasto SMART on openEHR
  slug: cadasto-smart-on-openehr
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadasto/refs/heads/main/openapi/cadasto-smart-on-openehr-openapi.json
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cadasto.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cadasto.io
  spf: true
hosts:
- cert_expires: Oct 26 04:05:16 2026 GMT
  host: www.cadasto.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 09:58:20 2026 GMT
  host: docs.cadasto.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.customer.cadasto.io
  https: false
kind: domain-security
layout: security
method: probed
name: Cadasto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cadasto, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Cadasto
provider_slug: cadasto
slug: cadasto-domain-security
source_filename: cadasto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cadasto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 04:05:16 2026 GMT\n  hsts: false\n- host: docs.cadasto.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 09:58:20 2026 GMT\n  hsts: false\n- host: api.customer.cadasto.io\n  https: false\ndomains:\n- domain: cadasto.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: cadasto.io\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cadasto/refs/heads/main/security/cadasto-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Healthcare
- Health IT
- openEHR
- Electronic Health Records
- Clinical Data Repository
- Interoperability
- FHIR
- Vendor Neutral Archive
- Clinical Data
- AQL
- MCP
- Agent Skills
- Netherlands
---
