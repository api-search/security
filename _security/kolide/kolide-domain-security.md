---
api_specs:
- filename: kolide-admin-users-api-openapi.yml
  format: yaml
  label: Kolide Admin Users API
  slug: kolide-admin-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/openapi/kolide-admin-users-api-openapi.yml
- filename: kolide-audit-logs-api-openapi.yml
  format: yaml
  label: Kolide Audit Logs API
  slug: kolide-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/openapi/kolide-audit-logs-api-openapi.yml
- filename: kolide-auth-logs-api-openapi.yml
  format: yaml
  label: Kolide Auth Logs API
  slug: kolide-auth-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/openapi/kolide-auth-logs-api-openapi.yml
- filename: kolide-checks-api-openapi.yml
  format: yaml
  label: Kolide Checks API
  slug: kolide-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/openapi/kolide-checks-api-openapi.yml
- filename: kolide-custom-check-drafts-api-openapi.yml
  format: yaml
  label: Kolide Custom Check Drafts API
  slug: kolide-custom-check-drafts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/openapi/kolide-custom-check-drafts-api-openapi.yml
- filename: kolide-deprovisioned-people-api-openapi.yml
  format: yaml
  label: Kolide Deprovisioned People API
  slug: kolide-deprovisioned-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/openapi/kolide-deprovisioned-people-api-openapi.yml
- filename: kolide-device-groups-api-openapi.yml
  format: yaml
  label: Kolide Device Groups API
  slug: kolide-device-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/openapi/kolide-device-groups-api-openapi.yml
- filename: kolide-devices-api-openapi.yml
  format: yaml
  label: Kolide Devices API
  slug: kolide-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/openapi/kolide-devices-api-openapi.yml
- filename: kolide-exemption-requests-api-openapi.yml
  format: yaml
  label: Kolide Exemption Requests API
  slug: kolide-exemption-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/openapi/kolide-exemption-requests-api-openapi.yml
- filename: kolide-issues-api-openapi.yml
  format: yaml
  label: Kolide Issues API
  slug: kolide-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/openapi/kolide-issues-api-openapi.yml
- filename: kolide-live-query-campaigns-api-openapi.yml
  format: yaml
  label: Kolide Live Query Campaigns API
  slug: kolide-live-query-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/openapi/kolide-live-query-campaigns-api-openapi.yml
- filename: kolide-packages-api-openapi.yml
  format: yaml
  label: Kolide Packages API
  slug: kolide-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/openapi/kolide-packages-api-openapi.yml
- filename: kolide-people-api-openapi.yml
  format: yaml
  label: Kolide People API
  slug: kolide-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/openapi/kolide-people-api-openapi.yml
- filename: kolide-person-groups-api-openapi.yml
  format: yaml
  label: Kolide Person Groups API
  slug: kolide-person-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/openapi/kolide-person-groups-api-openapi.yml
- filename: kolide-registration-requests-api-openapi.yml
  format: yaml
  label: Kolide Registration Requests API
  slug: kolide-registration-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/openapi/kolide-registration-requests-api-openapi.yml
- filename: kolide-reporting-api-openapi.yml
  format: yaml
  label: Kolide Reporting API
  slug: kolide-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/openapi/kolide-reporting-api-openapi.yml
- filename: kolide-whoami-api-openapi.yml
  format: yaml
  label: Kolide Whoami API
  slug: kolide-whoami-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/openapi/kolide-whoami-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kolide.com
  spf: true
hosts:
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: kolide.com
  hsts: true
  hsts_max_age: 631138519
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: api.kolide.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kolide Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kolide, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kolide
provider_slug: kolide
slug: kolide-domain-security
source_filename: kolide-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kolide.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 631138519\n- host: api.kolide.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: kolide.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kolide/refs/heads/main/security/kolide-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- B2B
- Security
- Device Trust
- Endpoint Security
- Zero Trust
- Compliance
- Identity
- osquery
- Device Management
---
