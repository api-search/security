---
api_specs:
- filename: aclaimant-answers-api-openapi.yml
  format: yaml
  label: Aclaimant Answers API
  slug: aclaimant-answers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aclaimant/refs/heads/main/openapi/aclaimant-answers-api-openapi.yml
- filename: aclaimant-bulk-api-openapi.yml
  format: yaml
  label: Aclaimant Bulk API
  slug: aclaimant-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aclaimant/refs/heads/main/openapi/aclaimant-bulk-api-openapi.yml
- filename: aclaimant-companies-api-openapi.yml
  format: yaml
  label: Aclaimant Companies API
  slug: aclaimant-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aclaimant/refs/heads/main/openapi/aclaimant-companies-api-openapi.yml
- filename: aclaimant-exposures-api-openapi.yml
  format: yaml
  label: Aclaimant Exposures API
  slug: aclaimant-exposures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aclaimant/refs/heads/main/openapi/aclaimant-exposures-api-openapi.yml
- filename: aclaimant-incidents-api-openapi.yml
  format: yaml
  label: Aclaimant Incidents API
  slug: aclaimant-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aclaimant/refs/heads/main/openapi/aclaimant-incidents-api-openapi.yml
- filename: aclaimant-policies-api-openapi.yml
  format: yaml
  label: Aclaimant Policies API
  slug: aclaimant-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aclaimant/refs/heads/main/openapi/aclaimant-policies-api-openapi.yml
- filename: aclaimant-policy-programs-api-openapi.yml
  format: yaml
  label: Aclaimant Policy Programs API
  slug: aclaimant-policy-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aclaimant/refs/heads/main/openapi/aclaimant-policy-programs-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aclaimant.com
  spf: true
hosts:
- cert_expires: Oct 24 13:48:54 2026 GMT
  host: www.aclaimant.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 15:39:07 2026 GMT
  host: api.aclaimant.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 15:39:07 2026 GMT
  host: developer.aclaimant.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Aclaimant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aclaimant, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Aclaimant
provider_slug: aclaimant
slug: aclaimant-domain-security
source_filename: aclaimant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aclaimant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 13:48:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.aclaimant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 15:39:07 2026 GMT\n  hsts: false\n- host: developer.aclaimant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 15:39:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aclaimant.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aclaimant/refs/heads/main/security/aclaimant-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Risk Management
- Insurance
- Claims Management
- Incident Management
- Safety
- RMIS
- Workers Compensation
- OSHA
- Enterprise Risk Management
- Insurtech
---
