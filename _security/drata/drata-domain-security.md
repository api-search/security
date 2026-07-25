---
api_specs:
- filename: drata-assets-api-openapi.yml
  format: yaml
  label: Drata Assets API
  slug: drata-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drata/refs/heads/main/openapi/drata-assets-api-openapi.yml
- filename: drata-audits-api-openapi.yml
  format: yaml
  label: Drata Audits API
  slug: drata-audits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drata/refs/heads/main/openapi/drata-audits-api-openapi.yml
- filename: drata-controls-api-openapi.yml
  format: yaml
  label: Drata Controls API
  slug: drata-controls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drata/refs/heads/main/openapi/drata-controls-api-openapi.yml
- filename: drata-evidence-library-api-openapi.yml
  format: yaml
  label: Drata Evidence Library API
  slug: drata-evidence-library-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drata/refs/heads/main/openapi/drata-evidence-library-api-openapi.yml
- filename: drata-frameworks-api-openapi.yml
  format: yaml
  label: Drata Frameworks API
  slug: drata-frameworks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drata/refs/heads/main/openapi/drata-frameworks-api-openapi.yml
- filename: drata-monitoring-tests-api-openapi.yml
  format: yaml
  label: Drata Monitoring Tests API
  slug: drata-monitoring-tests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drata/refs/heads/main/openapi/drata-monitoring-tests-api-openapi.yml
- filename: drata-personnel-api-openapi.yml
  format: yaml
  label: Drata Personnel API
  slug: drata-personnel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drata/refs/heads/main/openapi/drata-personnel-api-openapi.yml
- filename: drata-policies-api-openapi.yml
  format: yaml
  label: Drata Policies API
  slug: drata-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drata/refs/heads/main/openapi/drata-policies-api-openapi.yml
- filename: drata-risks-api-openapi.yml
  format: yaml
  label: Drata Risks API
  slug: drata-risks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drata/refs/heads/main/openapi/drata-risks-api-openapi.yml
- filename: drata-tasks-api-openapi.yml
  format: yaml
  label: Drata Tasks API
  slug: drata-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drata/refs/heads/main/openapi/drata-tasks-api-openapi.yml
- filename: drata-vendors-api-openapi.yml
  format: yaml
  label: Drata Vendors API
  slug: drata-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drata/refs/heads/main/openapi/drata-vendors-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: drata.com
  spf: true
hosts:
- cert_expires: Oct  7 03:49:09 2026 GMT
  host: drata.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 03:49:09 2026 GMT
  host: developers.drata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 03:49:09 2026 GMT
  host: public-api.drata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Drata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Drata, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Drata
provider_slug: drata
slug: drata-domain-security
source_filename: drata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: drata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 03:49:09 2026 GMT\n  hsts: null\n- host: developers.drata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 03:49:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: public-api.drata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 03:49:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: drata.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drata/refs/heads/main/security/drata-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- GRC
- Compliance
- SOC 2
- ISO 27001
- Security
---
