---
api_specs:
- filename: microsoft-security-response-center-msrc-acknowledgement-api-openapi.yml
  format: yaml
  label: Microsoft Security Response Center (MSRC) Acknowledgement API
  slug: microsoft-security-response-center-msrc-acknowledgement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-security-response-center-msrc/openapi/microsoft-security-response-center-msrc-acknowledgement-api-openapi.yml
- filename: microsoft-security-response-center-msrc-advisory-api-openapi.yml
  format: yaml
  label: Microsoft Security Response Center (MSRC) Advisory API
  slug: microsoft-security-response-center-msrc-advisory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-security-response-center-msrc/openapi/microsoft-security-response-center-msrc-advisory-api-openapi.yml
- filename: microsoft-security-response-center-msrc-affectedproduct-api-openapi.yml
  format: yaml
  label: Microsoft Security Response Center (MSRC) Affected Product API
  slug: microsoft-security-response-center-msrc-affectedproduct-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-security-response-center-msrc/openapi/microsoft-security-response-center-msrc-affectedproduct-api-openapi.yml
- filename: microsoft-security-response-center-msrc-csaf-api-openapi.yml
  format: yaml
  label: Microsoft Security Response Center (MSRC) Csaf API
  slug: microsoft-security-response-center-msrc-csaf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-security-response-center-msrc/openapi/microsoft-security-response-center-msrc-csaf-api-openapi.yml
- filename: microsoft-security-response-center-msrc-cvrf-api-openapi.yml
  format: yaml
  label: Microsoft Security Response Center (MSRC) Cvrf API
  slug: microsoft-security-response-center-msrc-cvrf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-security-response-center-msrc/openapi/microsoft-security-response-center-msrc-cvrf-api-openapi.yml
- filename: microsoft-security-response-center-msrc-deployment-api-openapi.yml
  format: yaml
  label: Microsoft Security Response Center (MSRC) Deployment API
  slug: microsoft-security-response-center-msrc-deployment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-security-response-center-msrc/openapi/microsoft-security-response-center-msrc-deployment-api-openapi.yml
- filename: microsoft-security-response-center-msrc-headercontent-api-openapi.yml
  format: yaml
  label: Microsoft Security Response Center (MSRC) Header Content API
  slug: microsoft-security-response-center-msrc-headercontent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-security-response-center-msrc/openapi/microsoft-security-response-center-msrc-headercontent-api-openapi.yml
- filename: microsoft-security-response-center-msrc-metadata-api-openapi.yml
  format: yaml
  label: Microsoft Security Response Center (MSRC) Metadata API
  slug: microsoft-security-response-center-msrc-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-security-response-center-msrc/openapi/microsoft-security-response-center-msrc-metadata-api-openapi.yml
- filename: microsoft-security-response-center-msrc-releasenote-api-openapi.yml
  format: yaml
  label: Microsoft Security Response Center (MSRC) Release Note API
  slug: microsoft-security-response-center-msrc-releasenote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-security-response-center-msrc/openapi/microsoft-security-response-center-msrc-releasenote-api-openapi.yml
- filename: microsoft-security-response-center-msrc-revisionnote-api-openapi.yml
  format: yaml
  label: Microsoft Security Response Center (MSRC) Revision Note API
  slug: microsoft-security-response-center-msrc-revisionnote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-security-response-center-msrc/openapi/microsoft-security-response-center-msrc-revisionnote-api-openapi.yml
- filename: microsoft-security-response-center-msrc-updates-api-openapi.yml
  format: yaml
  label: Microsoft Security Response Center (MSRC) Updates API
  slug: microsoft-security-response-center-msrc-updates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-security-response-center-msrc/openapi/microsoft-security-response-center-msrc-updates-api-openapi.yml
- filename: microsoft-security-response-center-msrc-vulnerability-api-openapi.yml
  format: yaml
  label: Microsoft Security Response Center (MSRC) Vulnerability API
  slug: microsoft-security-response-center-msrc-vulnerability-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-security-response-center-msrc/openapi/microsoft-security-response-center-msrc-vulnerability-api-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Nov 17 16:33:21 2026 GMT
  host: msrc.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Microsoft Security Response Center Msrc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Security Response Center (MSRC), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Security Response Center (MSRC)
provider_slug: microsoft-security-response-center-msrc
slug: microsoft-security-response-center-msrc-domain-security
source_filename: microsoft-security-response-center-msrc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: msrc.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 16:33:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/microsoft-security-response-center-msrc/security/microsoft-security-response-center-msrc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CSAF
- CVRF
- OData
- Public APIs
- Security
- Security Updates
- Vulnerabilities
---
