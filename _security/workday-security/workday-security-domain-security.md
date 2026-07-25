---
api_specs:
- filename: workday-security-account-signons-api-openapi.yml
  format: yaml
  label: Workday Security Account Signons API
  slug: workday-security-account-signons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-security/refs/heads/main/openapi/workday-security-account-signons-api-openapi.yml
- filename: workday-security-audit-logs-api-openapi.yml
  format: yaml
  label: Workday Security Audit Logs API
  slug: workday-security-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-security/refs/heads/main/openapi/workday-security-audit-logs-api-openapi.yml
- filename: workday-security-authentication-configuration-api-openapi.yml
  format: yaml
  label: Workday Security Authentication Configuration API
  slug: workday-security-authentication-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-security/refs/heads/main/openapi/workday-security-authentication-configuration-api-openapi.yml
- filename: workday-security-compliance-reports-api-openapi.yml
  format: yaml
  label: Workday Security Compliance Reports API
  slug: workday-security-compliance-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-security/refs/heads/main/openapi/workday-security-compliance-reports-api-openapi.yml
- filename: workday-security-domain-security-policies-api-openapi.yml
  format: yaml
  label: Workday Security Domain Security Policies API
  slug: workday-security-domain-security-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-security/refs/heads/main/openapi/workday-security-domain-security-policies-api-openapi.yml
- filename: workday-security-oauth-tokens-api-openapi.yml
  format: yaml
  label: Workday Security OAuth Tokens API
  slug: workday-security-oauth-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-security/refs/heads/main/openapi/workday-security-oauth-tokens-api-openapi.yml
- filename: workday-security-security-audit-api-openapi.yml
  format: yaml
  label: Workday Security Security Audit API
  slug: workday-security-security-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-security/refs/heads/main/openapi/workday-security-security-audit-api-openapi.yml
- filename: workday-security-security-group-members-api-openapi.yml
  format: yaml
  label: Workday Security Security Group Members API
  slug: workday-security-security-group-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-security/refs/heads/main/openapi/workday-security-security-group-members-api-openapi.yml
- filename: workday-security-security-groups-api-openapi.yml
  format: yaml
  label: Workday Security Security Groups API
  slug: workday-security-security-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-security/refs/heads/main/openapi/workday-security-security-groups-api-openapi.yml
- filename: workday-security-sessions-api-openapi.yml
  format: yaml
  label: Workday Security Sessions API
  slug: workday-security-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-security/refs/heads/main/openapi/workday-security-sessions-api-openapi.yml
- filename: workday-security-unidentified-signons-api-openapi.yml
  format: yaml
  label: Workday Security Unidentified Signons API
  slug: workday-security-unidentified-signons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-security/refs/heads/main/openapi/workday-security-unidentified-signons-api-openapi.yml
- filename: workday-security-user-accounts-api-openapi.yml
  format: yaml
  label: Workday Security User Accounts API
  slug: workday-security-user-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-security/refs/heads/main/openapi/workday-security-user-accounts-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: workday.com
  spf: true
hosts:
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: community.workday.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: www.workday.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 03:30:49 2026 GMT
  host: wd2-impl-services1.workday.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Workday Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Workday Security, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Workday Security
provider_slug: workday-security
slug: workday-security-domain-security
source_filename: workday-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: community.workday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: null\n- host: www.workday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: wd2-impl-services1.workday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 03:30:49 2026 GMT\n  hsts: null\ndomains:\n- domain: workday.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-security/refs/heads/main/security/workday-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Access Control
- Audit
- Authentication
- Compliance
- Enterprise
- Identity Management
- Privacy
- SAML
- Security
- SSO
---
