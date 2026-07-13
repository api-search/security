---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: SailPoint Identity Security Cloud V3 API
  slug: identity-security-cloud-v3-api
  spec_type: OpenAPI
  url: https://developer.sailpoint.com/docs/api/v3/identity-security-cloud-v-3-api/
- filename: openapi.yaml
  format: yaml
  label: SailPoint Identity Security Cloud V2024 API
  slug: identity-security-cloud-v2024-api
  spec_type: OpenAPI
  url: https://developer.sailpoint.com/docs/api/v2024/identity-security-cloud-v-2024-api/
- filename: openapi.yaml
  format: yaml
  label: SailPoint Identity Security Cloud V2025 API
  slug: identity-security-cloud-v2025-api
  spec_type: OpenAPI
  url: https://developer.sailpoint.com/docs/api/v2025/identity-security-cloud-v-2025-api/
- filename: openapi.yaml
  format: yaml
  label: SailPoint Identity Security Cloud Beta API
  slug: identity-security-cloud-beta-api
  spec_type: OpenAPI
  url: https://developer.sailpoint.com/docs/api/beta/identity-security-cloud-beta-api/
- filename: openapi.yaml
  format: yaml
  label: SailPoint IdentityIQ SCIM API
  slug: identityiq-scim-api
  spec_type: OpenAPI
  url: https://developer.sailpoint.com/docs/api/iiq/identityiq-scim-rest-api/
- filename: openapi.yaml
  format: yaml
  label: SailPoint Identity Security Cloud V2026 API
  slug: identity-security-cloud-v2026-api
  spec_type: OpenAPI
  url: https://developer.sailpoint.com/docs/api/v2026/identity-security-cloud-v-2026-api/
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazonaws.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sailpoint.com
  spf: true
hosts:
- cert_expires: Oct  8 05:58:36 2026 GMT
  host: developer.sailpoint.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sailpoint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SailPoint, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SailPoint
provider_slug: sailpoint
slug: sailpoint-domain-security
source_filename: sailpoint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.sailpoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 05:58:36 2026 GMT\n  hsts: false\ndomains:\n- domain: sailpoint.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sailpoint/refs/heads/main/security/sailpoint-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Access Governance
- Compliance
- IAM
- Identity Management
- Identity Security
- Security
---
