---
api_specs:
- filename: upwind-access-management-api-openapi.yml
  format: yaml
  label: Upwind access-management API
  slug: upwind-access-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/openapi/upwind-access-management-api-openapi.yml
- filename: upwind-api-security-api-openapi.yml
  format: yaml
  label: Upwind api-security API
  slug: upwind-api-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/openapi/upwind-api-security-api-openapi.yml
- filename: upwind-cloud-accounts-api-openapi.yml
  format: yaml
  label: Upwind cloud-accounts API
  slug: upwind-cloud-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/openapi/upwind-cloud-accounts-api-openapi.yml
- filename: upwind-configurations-api-openapi.yml
  format: yaml
  label: Upwind configurations API
  slug: upwind-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/openapi/upwind-configurations-api-openapi.yml
- filename: upwind-events-api-openapi.yml
  format: yaml
  label: Upwind events API
  slug: upwind-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/openapi/upwind-events-api-openapi.yml
- filename: upwind-integrations-api-openapi.yml
  format: yaml
  label: Upwind integrations API
  slug: upwind-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/openapi/upwind-integrations-api-openapi.yml
- filename: upwind-inventory-api-openapi.yml
  format: yaml
  label: Upwind Inventory API
  slug: upwind-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/openapi/upwind-inventory-api-openapi.yml
- filename: upwind-packages-api-openapi.yml
  format: yaml
  label: Upwind packages API
  slug: upwind-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/openapi/upwind-packages-api-openapi.yml
- filename: upwind-shiftleft-api-openapi.yml
  format: yaml
  label: Upwind shiftleft API
  slug: upwind-shiftleft-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/openapi/upwind-shiftleft-api-openapi.yml
- filename: upwind-threats-api-openapi.yml
  format: yaml
  label: Upwind threats API
  slug: upwind-threats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/openapi/upwind-threats-api-openapi.yml
- filename: upwind-vulnerabilities-api-openapi.yml
  format: yaml
  label: Upwind vulnerabilities API
  slug: upwind-vulnerabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/openapi/upwind-vulnerabilities-api-openapi.yml
- filename: upwind-workflows-api-openapi.yml
  format: yaml
  label: Upwind workflows API
  slug: upwind-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/openapi/upwind-workflows-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: upwind.io
  spf: true
hosts:
- cert_expires: Sep 15 21:02:27 2026 GMT
  host: upwind.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: api.upwind.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 23:59:59 2026 GMT
  host: api.eu.upwind.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Upwind Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Upwind, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Upwind
provider_slug: upwind
slug: upwind-domain-security
source_filename: upwind-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: upwind.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 21:02:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.upwind.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: null\n- host: api.eu.upwind.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: upwind.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/security/upwind-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Security
- Cloud Security
- CNAPP
- Vulnerability Management
- Container Security
- Kubernetes
- API Security
- Threat Detection
- Data Security
---
