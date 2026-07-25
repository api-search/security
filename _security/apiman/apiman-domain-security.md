---
api_specs:
- filename: apiman-actions-api-openapi.yml
  format: yaml
  label: Apiman Actions API
  slug: apiman-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiman/refs/heads/main/openapi/apiman-actions-api-openapi.yml
- filename: apiman-blobs-api-openapi.yml
  format: yaml
  label: Apiman Blobs API
  slug: apiman-blobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiman/refs/heads/main/openapi/apiman-blobs-api-openapi.yml
- filename: apiman-developers-api-openapi.yml
  format: yaml
  label: Apiman Developers API
  slug: apiman-developers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiman/refs/heads/main/openapi/apiman-developers-api-openapi.yml
- filename: apiman-devportal-api-openapi.yml
  format: yaml
  label: Apiman Devportal API
  slug: apiman-devportal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiman/refs/heads/main/openapi/apiman-devportal-api-openapi.yml
- filename: apiman-downloads-api-openapi.yml
  format: yaml
  label: Apiman Downloads API
  slug: apiman-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiman/refs/heads/main/openapi/apiman-downloads-api-openapi.yml
- filename: apiman-events-api-openapi.yml
  format: yaml
  label: Apiman Events API
  slug: apiman-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiman/refs/heads/main/openapi/apiman-events-api-openapi.yml
- filename: apiman-experimental-api-openapi.yml
  format: yaml
  label: Apiman Experimental API
  slug: apiman-experimental-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiman/refs/heads/main/openapi/apiman-experimental-api-openapi.yml
- filename: apiman-gateways-api-openapi.yml
  format: yaml
  label: Apiman Gateways API
  slug: apiman-gateways-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiman/refs/heads/main/openapi/apiman-gateways-api-openapi.yml
- filename: apiman-organizations-api-openapi.yml
  format: yaml
  label: Apiman Organizations API
  slug: apiman-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiman/refs/heads/main/openapi/apiman-organizations-api-openapi.yml
- filename: apiman-plugins-api-openapi.yml
  format: yaml
  label: Apiman Plugins API
  slug: apiman-plugins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiman/refs/heads/main/openapi/apiman-plugins-api-openapi.yml
- filename: apiman-policy-definitions-api-openapi.yml
  format: yaml
  label: Apiman Policy Definitions API
  slug: apiman-policy-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiman/refs/heads/main/openapi/apiman-policy-definitions-api-openapi.yml
- filename: apiman-roles-api-openapi.yml
  format: yaml
  label: Apiman Roles API
  slug: apiman-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiman/refs/heads/main/openapi/apiman-roles-api-openapi.yml
- filename: apiman-search-api-openapi.yml
  format: yaml
  label: Apiman Search API
  slug: apiman-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiman/refs/heads/main/openapi/apiman-search-api-openapi.yml
- filename: apiman-system-api-openapi.yml
  format: yaml
  label: Apiman System API
  slug: apiman-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiman/refs/heads/main/openapi/apiman-system-api-openapi.yml
- filename: apiman-users-api-openapi.yml
  format: yaml
  label: Apiman Users API
  slug: apiman-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiman/refs/heads/main/openapi/apiman-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apiman.io
  spf: true
hosts:
- cert_expires: Sep 20 19:26:22 2026 GMT
  host: www.apiman.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apiman Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apiman, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Apiman
provider_slug: apiman
slug: apiman-domain-security
source_filename: apiman-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apiman.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 19:26:22 2026 GMT\n  hsts: false\ndomains:\n- domain: apiman.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apiman/refs/heads/main/security/apiman-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- API Gateway
- API Management
- Developer Portal
- Java
- Open Source
---
