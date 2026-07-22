---
api_specs:
- filename: scoutrfp-suppliers-v1-openapi.json
  format: json
  label: Workday Strategic Sourcing - Suppliers API
  slug: workday-strategic-sourcing-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scoutrfp/refs/heads/main/openapi/scoutrfp-suppliers-v1-openapi.json
- filename: scoutrfp-events-v1-openapi.json
  format: json
  label: Workday Strategic Sourcing - Events API
  slug: workday-strategic-sourcing-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scoutrfp/refs/heads/main/openapi/scoutrfp-events-v1-openapi.json
- filename: scoutrfp-reports-v1-openapi.json
  format: json
  label: Workday Strategic Sourcing - Reports API
  slug: workday-strategic-sourcing-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scoutrfp/refs/heads/main/openapi/scoutrfp-reports-v1-openapi.json
- filename: scoutrfp-contracts-v1-openapi.json
  format: json
  label: Workday Strategic Sourcing - Contracts API
  slug: workday-strategic-sourcing-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scoutrfp/refs/heads/main/openapi/scoutrfp-contracts-v1-openapi.json
- filename: scoutrfp-projects-v1-openapi.json
  format: json
  label: Workday Strategic Sourcing - Projects API
  slug: workday-strategic-sourcing-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scoutrfp/refs/heads/main/openapi/scoutrfp-projects-v1-openapi.json
- filename: scoutrfp-payments-v1-openapi.json
  format: json
  label: Workday Strategic Sourcing - Payments API
  slug: workday-strategic-sourcing-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scoutrfp/refs/heads/main/openapi/scoutrfp-payments-v1-openapi.json
- filename: scoutrfp-fields-v1-openapi.json
  format: json
  label: Workday Strategic Sourcing - Fields API
  slug: workday-strategic-sourcing-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scoutrfp/refs/heads/main/openapi/scoutrfp-fields-v1-openapi.json
- filename: scoutrfp-awards-v1-openapi.json
  format: json
  label: Workday Strategic Sourcing - Awards API
  slug: workday-strategic-sourcing-awards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scoutrfp/refs/heads/main/openapi/scoutrfp-awards-v1-openapi.json
- filename: scoutrfp-attachments-v1-openapi.json
  format: json
  label: Workday Strategic Sourcing - Attachments API
  slug: workday-strategic-sourcing-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scoutrfp/refs/heads/main/openapi/scoutrfp-attachments-v1-openapi.json
- filename: scoutrfp-spend_categories-v1-openapi.json
  format: json
  label: Workday Strategic Sourcing - Spend Categories API
  slug: workday-strategic-sourcing-spend-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scoutrfp/refs/heads/main/openapi/scoutrfp-spend_categories-v1-openapi.json
- filename: scoutrfp-scim-v2-openapi.json
  format: json
  label: Workday Strategic Sourcing - SCIM (Users) API
  slug: workday-strategic-sourcing-scim-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scoutrfp/refs/heads/main/openapi/scoutrfp-scim-v2-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: workday.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: workdayspend.com
  spf: false
hosts:
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: www.workday.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 16 23:59:59 2026 GMT
  host: apidocs.workdayspend.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: api.us.workdayspend.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scoutrfp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scout RFP (Workday Strategic Sourcing), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Scout RFP (Workday Strategic Sourcing)
provider_slug: scoutrfp
slug: scoutrfp-domain-security
source_filename: scoutrfp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.workday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apidocs.workdayspend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 23:59:59 2026 GMT\n  hsts: false\n- host: api.us.workdayspend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: workday.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: workdayspend.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scoutrfp/refs/heads/main/security/scoutrfp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Procurement
- Strategic Sourcing
- Supplier Management
- Spend Management
- RFP
- Contracts
- SCIM
- JSON:API
---
