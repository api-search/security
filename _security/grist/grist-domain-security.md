---
api_specs:
- filename: grist-attachments-api-openapi.yml
  format: yaml
  label: Grist Attachments API
  slug: grist-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grist/refs/heads/main/openapi/grist-attachments-api-openapi.yml
- filename: grist-columns-api-openapi.yml
  format: yaml
  label: Grist Columns API
  slug: grist-columns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grist/refs/heads/main/openapi/grist-columns-api-openapi.yml
- filename: grist-data-api-openapi.yml
  format: yaml
  label: Grist Data API
  slug: grist-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grist/refs/heads/main/openapi/grist-data-api-openapi.yml
- filename: grist-docs-api-openapi.yml
  format: yaml
  label: Grist Docs API
  slug: grist-docs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grist/refs/heads/main/openapi/grist-docs-api-openapi.yml
- filename: grist-forms-api-openapi.yml
  format: yaml
  label: Grist Forms API
  slug: grist-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grist/refs/heads/main/openapi/grist-forms-api-openapi.yml
- filename: grist-orgs-api-openapi.yml
  format: yaml
  label: Grist Orgs API
  slug: grist-orgs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grist/refs/heads/main/openapi/grist-orgs-api-openapi.yml
- filename: grist-profile-api-openapi.yml
  format: yaml
  label: Grist Profile API
  slug: grist-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grist/refs/heads/main/openapi/grist-profile-api-openapi.yml
- filename: grist-records-api-openapi.yml
  format: yaml
  label: Grist Records API
  slug: grist-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grist/refs/heads/main/openapi/grist-records-api-openapi.yml
- filename: grist-service-accounts-api-openapi.yml
  format: yaml
  label: Grist service accounts API
  slug: grist-service-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grist/refs/heads/main/openapi/grist-service-accounts-api-openapi.yml
- filename: grist-session-api-openapi.yml
  format: yaml
  label: Grist Session API
  slug: grist-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grist/refs/heads/main/openapi/grist-session-api-openapi.yml
- filename: grist-sql-api-openapi.yml
  format: yaml
  label: Grist Sql API
  slug: grist-sql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grist/refs/heads/main/openapi/grist-sql-api-openapi.yml
- filename: grist-tables-api-openapi.yml
  format: yaml
  label: Grist Tables API
  slug: grist-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grist/refs/heads/main/openapi/grist-tables-api-openapi.yml
- filename: grist-templates-api-openapi.yml
  format: yaml
  label: Grist Templates API
  slug: grist-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grist/refs/heads/main/openapi/grist-templates-api-openapi.yml
- filename: grist-users-api-openapi.yml
  format: yaml
  label: Grist Users API
  slug: grist-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grist/refs/heads/main/openapi/grist-users-api-openapi.yml
- filename: grist-webhooks-api-openapi.yml
  format: yaml
  label: Grist Webhooks API
  slug: grist-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grist/refs/heads/main/openapi/grist-webhooks-api-openapi.yml
- filename: grist-widgets-api-openapi.yml
  format: yaml
  label: Grist Widgets API
  slug: grist-widgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grist/refs/heads/main/openapi/grist-widgets-api-openapi.yml
- filename: grist-workspaces-api-openapi.yml
  format: yaml
  label: Grist Workspaces API
  slug: grist-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grist/refs/heads/main/openapi/grist-workspaces-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getgrist.com
  spf: true
hosts:
- cert_expires: Oct  7 08:51:50 2026 GMT
  host: www.getgrist.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 14:16:48 2026 GMT
  host: support.getgrist.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: docs.getgrist.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Grist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Grist, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Grist
provider_slug: grist
slug: grist-domain-security
source_filename: grist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getgrist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 08:51:50 2026 GMT\n  hsts: false\n- host: support.getgrist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 14:16:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: docs.getgrist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: getgrist.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grist/refs/heads/main/security/grist-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Spreadsheets
- Database
- Collaboration
- No-Code
- Data Management
- Webhook
- Open Source
---
