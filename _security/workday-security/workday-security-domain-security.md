---
api_specs:
- filename: Authentication_OpenAPI.json
  format: json
  label: Workday Authentication API
  slug: workday-authentication-api
  spec_type: OpenAPI
  url: https://community.workday.com/sites/default/files/file-hosting/productionapi/Security/v44.0/Authentication_OpenAPI.json
- filename: Identity_Management_OpenAPI.json
  format: json
  label: Workday Identity Management API
  slug: workday-identity-management-api
  spec_type: OpenAPI
  url: https://community.workday.com/sites/default/files/file-hosting/productionapi/Security/v44.0/Identity_Management_OpenAPI.json
- filename: Security_Groups_OpenAPI.json
  format: json
  label: Workday Security Groups API
  slug: workday-security-groups-api
  spec_type: OpenAPI
  url: https://community.workday.com/sites/default/files/file-hosting/productionapi/Security/v44.0/Security_Groups_OpenAPI.json
- filename: Audit_OpenAPI.json
  format: json
  label: Workday Audit and Compliance API
  slug: workday-audit-and-compliance-api
  spec_type: OpenAPI
  url: https://community.workday.com/sites/default/files/file-hosting/productionapi/Security/v44.0/Audit_OpenAPI.json
- filename: Privacy_OpenAPI.json
  format: json
  label: Workday Privacy API
  slug: workday-privacy-api
  spec_type: OpenAPI
  url: https://community.workday.com/sites/default/files/file-hosting/productionapi/Security/v44.0/Privacy_OpenAPI.json
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
