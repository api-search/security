---
api_specs:
- filename: cove.tool-authentication-token-api-openapi.yml
  format: yaml
  label: Cove.Tool Authentication Token API
  slug: cove.tool-authentication-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cove.tool/refs/heads/main/openapi/cove.tool-authentication-token-api-openapi.yml
- filename: cove.tool-daylight-analysis-api-openapi.yml
  format: yaml
  label: Cove.Tool Daylight Analysis API
  slug: cove.tool-daylight-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cove.tool/refs/heads/main/openapi/cove.tool-daylight-analysis-api-openapi.yml
- filename: cove.tool-energy-codes-api-openapi.yml
  format: yaml
  label: Cove.Tool Energy Codes API
  slug: cove.tool-energy-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cove.tool/refs/heads/main/openapi/cove.tool-energy-codes-api-openapi.yml
- filename: cove.tool-profiles-api-openapi.yml
  format: yaml
  label: Cove.Tool Profiles API
  slug: cove.tool-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cove.tool/refs/heads/main/openapi/cove.tool-profiles-api-openapi.yml
- filename: cove.tool-project-geometry-api-openapi.yml
  format: yaml
  label: Cove.Tool Project Geometry API
  slug: cove.tool-project-geometry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cove.tool/refs/heads/main/openapi/cove.tool-project-geometry-api-openapi.yml
- filename: cove.tool-projects-api-openapi.yml
  format: yaml
  label: Cove.Tool Projects API
  slug: cove.tool-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cove.tool/refs/heads/main/openapi/cove.tool-projects-api-openapi.yml
- filename: cove.tool-user-api-openapi.yml
  format: yaml
  label: Cove.Tool User API
  slug: cove.tool-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cove.tool/refs/heads/main/openapi/cove.tool-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cove.inc
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: covetool.com
  spf: true
hosts:
- cert_expires: Nov  6 23:03:07 2026 GMT
  host: cove.inc
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 12:34:42 2026 GMT
  host: developers.covetool.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep  3 23:59:59 2026 GMT
  host: app.covetool.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Cove.Tool Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cove.Tool, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cove.Tool
provider_slug: cove.tool
slug: cove.tool-domain-security
source_filename: cove.tool-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cove.inc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:03:07 2026 GMT\n  hsts: false\n- host: developers.covetool.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 23 12:34:42 2026 GMT\n  hsts: false\n- host: app.covetool.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  3 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: cove.inc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: covetool.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cove.tool/refs/heads/main/security/cove.tool-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Building Performance
- Energy Modeling
- Daylight Analysis
- Sustainability
- Architecture
- AEC
- Simulation
- Embodied Carbon
- Building Design
---
