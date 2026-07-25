---
api_specs:
- filename: useparagon-actionkit-api-openapi.yml
  format: yaml
  label: Paragon ActionKit API
  slug: useparagon-actionkit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useparagon/refs/heads/main/openapi/useparagon-actionkit-api-openapi.yml
- filename: useparagon-connect-api-openapi.yml
  format: yaml
  label: Paragon Connect API
  slug: useparagon-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useparagon/refs/heads/main/openapi/useparagon-connect-api-openapi.yml
- filename: useparagon-integrations-api-openapi.yml
  format: yaml
  label: Paragon Integrations API
  slug: useparagon-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useparagon/refs/heads/main/openapi/useparagon-integrations-api-openapi.yml
- filename: useparagon-managed-sync-api-openapi.yml
  format: yaml
  label: Paragon Managed Sync API
  slug: useparagon-managed-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useparagon/refs/heads/main/openapi/useparagon-managed-sync-api-openapi.yml
- filename: useparagon-permissions-api-openapi.yml
  format: yaml
  label: Paragon Permissions API
  slug: useparagon-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useparagon/refs/heads/main/openapi/useparagon-permissions-api-openapi.yml
- filename: useparagon-proxy-api-openapi.yml
  format: yaml
  label: Paragon Proxy API
  slug: useparagon-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useparagon/refs/heads/main/openapi/useparagon-proxy-api-openapi.yml
- filename: useparagon-users-api-openapi.yml
  format: yaml
  label: Paragon Users API
  slug: useparagon-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useparagon/refs/heads/main/openapi/useparagon-users-api-openapi.yml
- filename: useparagon-workflows-api-openapi.yml
  format: yaml
  label: Paragon Workflows API
  slug: useparagon-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/useparagon/refs/heads/main/openapi/useparagon-workflows-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: useparagon.com
  spf: true
hosts:
- cert_expires: Sep  8 23:59:59 2026 GMT
  host: www.useparagon.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 00:16:04 2026 GMT
  host: docs.useparagon.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 05:33:24 2026 GMT
  host: zeus.useparagon.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Useparagon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paragon, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Paragon
provider_slug: useparagon
slug: useparagon-domain-security
source_filename: useparagon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.useparagon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.useparagon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 00:16:04 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: zeus.useparagon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 05:33:24 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: useparagon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/useparagon/refs/heads/main/security/useparagon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Integration
- iPaaS
- Embedded Integrations
- Workflows
- ActionKit
- Managed Sync
- AI Agents
---
