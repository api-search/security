---
api_specs:
- filename: infra-authentication-api-openapi.yml
  format: yaml
  label: Infra Authentication API
  slug: infra-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infra/refs/heads/main/openapi/infra-authentication-api-openapi.yml
- filename: infra-destinations-api-openapi.yml
  format: yaml
  label: Infra Destinations API
  slug: infra-destinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infra/refs/heads/main/openapi/infra-destinations-api-openapi.yml
- filename: infra-grants-api-openapi.yml
  format: yaml
  label: Infra Grants API
  slug: infra-grants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infra/refs/heads/main/openapi/infra-grants-api-openapi.yml
- filename: infra-groups-api-openapi.yml
  format: yaml
  label: Infra Groups API
  slug: infra-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infra/refs/heads/main/openapi/infra-groups-api-openapi.yml
- filename: infra-organizations-api-openapi.yml
  format: yaml
  label: Infra Organizations API
  slug: infra-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infra/refs/heads/main/openapi/infra-organizations-api-openapi.yml
- filename: infra-providers-api-openapi.yml
  format: yaml
  label: Infra Providers API
  slug: infra-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infra/refs/heads/main/openapi/infra-providers-api-openapi.yml
- filename: infra-settings-api-openapi.yml
  format: yaml
  label: Infra Settings API
  slug: infra-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infra/refs/heads/main/openapi/infra-settings-api-openapi.yml
- filename: infra-users-api-openapi.yml
  format: yaml
  label: Infra Users API
  slug: infra-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infra/refs/heads/main/openapi/infra-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: infrahq.com
  spf: true
hosts:
- cert_expires: Oct  9 21:53:46 2026 GMT
  host: infrahq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.infrahq.com
  https: false
kind: domain-security
layout: security
method: probed
name: Infra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Infra, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Infra
provider_slug: infra
slug: infra-domain-security
source_filename: infra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: infrahq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 21:53:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.infrahq.com\n  https: false\ndomains:\n- domain: infrahq.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infra/refs/heads/main/security/infra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Identity
- Access Management
- Authentication
- Authorization
- Infrastructure
- Kubernetes
- OIDC
- Security
- Open-Source
---
