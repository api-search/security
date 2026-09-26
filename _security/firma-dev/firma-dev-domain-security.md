---
api_specs:
- filename: firma-dev-company-api-openapi.yml
  format: yaml
  label: Firma.dev Company API
  slug: firma-dev-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firma-dev/refs/heads/main/openapi/firma-dev-company-api-openapi.yml
- filename: firma-dev-custom-fields-api-openapi.yml
  format: yaml
  label: Firma.dev Custom Fields API
  slug: firma-dev-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firma-dev/refs/heads/main/openapi/firma-dev-custom-fields-api-openapi.yml
- filename: firma-dev-email-domains-api-openapi.yml
  format: yaml
  label: Firma.dev Email Domains API
  slug: firma-dev-email-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firma-dev/refs/heads/main/openapi/firma-dev-email-domains-api-openapi.yml
- filename: firma-dev-email-templates-api-openapi.yml
  format: yaml
  label: Firma.dev Email Templates API
  slug: firma-dev-email-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firma-dev/refs/heads/main/openapi/firma-dev-email-templates-api-openapi.yml
- filename: firma-dev-jwt-management-api-openapi.yml
  format: yaml
  label: Firma.dev JWT Management API
  slug: firma-dev-jwt-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firma-dev/refs/heads/main/openapi/firma-dev-jwt-management-api-openapi.yml
- filename: firma-dev-organization-seals-api-openapi.yml
  format: yaml
  label: Firma.dev Organization Seals API
  slug: firma-dev-organization-seals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firma-dev/refs/heads/main/openapi/firma-dev-organization-seals-api-openapi.yml
- filename: firma-dev-signer-terms-api-openapi.yml
  format: yaml
  label: Firma.dev Signer Terms API
  slug: firma-dev-signer-terms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firma-dev/refs/heads/main/openapi/firma-dev-signer-terms-api-openapi.yml
- filename: firma-dev-signing-requests-api-openapi.yml
  format: yaml
  label: Firma.dev Signing Requests API
  slug: firma-dev-signing-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firma-dev/refs/heads/main/openapi/firma-dev-signing-requests-api-openapi.yml
- filename: firma-dev-templates-api-openapi.yml
  format: yaml
  label: Firma.dev Templates API
  slug: firma-dev-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firma-dev/refs/heads/main/openapi/firma-dev-templates-api-openapi.yml
- filename: firma-dev-webhooks-api-openapi.yml
  format: yaml
  label: Firma.dev Webhooks API
  slug: firma-dev-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firma-dev/refs/heads/main/openapi/firma-dev-webhooks-api-openapi.yml
- filename: firma-dev-workspace-settings-api-openapi.yml
  format: yaml
  label: Firma.dev Workspace Settings API
  slug: firma-dev-workspace-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firma-dev/refs/heads/main/openapi/firma-dev-workspace-settings-api-openapi.yml
- filename: firma-dev-workspaces-api-openapi.yml
  format: yaml
  label: Firma.dev Workspaces API
  slug: firma-dev-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firma-dev/refs/heads/main/openapi/firma-dev-workspaces-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: firma.dev
  spf: true
hosts:
- cert_expires: Dec 20 06:57:26 2026 GMT
  host: firma.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 22 06:45:11 2026 GMT
  host: api.firma.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Firma Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Firma.dev, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Firma.dev
provider_slug: firma-dev
slug: firma-dev-domain-security
source_filename: firma-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: firma.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 06:57:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.firma.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 06:45:11 2026 GMT\n  hsts: null\ndomains:\n- domain: firma.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/firma-dev/refs/heads/main/security/firma-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- eSignature
- API
- DeveloperTools
- LowCost
- WhiteLabel
---
