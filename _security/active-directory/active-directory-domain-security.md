---
api_specs:
- filename: active-directory-app-role-assignments-api-openapi.yml
  format: yaml
  label: Microsoft Active Directory App Role Assignments API
  slug: active-directory-app-role-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/active-directory/refs/heads/main/openapi/active-directory-app-role-assignments-api-openapi.yml
- filename: active-directory-applications-api-openapi.yml
  format: yaml
  label: Microsoft Active Directory Applications API
  slug: active-directory-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/active-directory/refs/heads/main/openapi/active-directory-applications-api-openapi.yml
- filename: active-directory-groups-api-openapi.yml
  format: yaml
  label: Microsoft Active Directory Groups API
  slug: active-directory-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/active-directory/refs/heads/main/openapi/active-directory-groups-api-openapi.yml
- filename: active-directory-members-api-openapi.yml
  format: yaml
  label: Microsoft Active Directory Members API
  slug: active-directory-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/active-directory/refs/heads/main/openapi/active-directory-members-api-openapi.yml
- filename: active-directory-owners-api-openapi.yml
  format: yaml
  label: Microsoft Active Directory Owners API
  slug: active-directory-owners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/active-directory/refs/heads/main/openapi/active-directory-owners-api-openapi.yml
- filename: active-directory-service-principals-api-openapi.yml
  format: yaml
  label: Microsoft Active Directory Service Principals API
  slug: active-directory-service-principals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/active-directory/refs/heads/main/openapi/active-directory-service-principals-api-openapi.yml
- filename: active-directory-users-api-openapi.yml
  format: yaml
  label: Microsoft Active Directory Users API
  slug: active-directory-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/active-directory/refs/heads/main/openapi/active-directory-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Nov 20 02:11:36 2026 GMT
  host: developer.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: graph.microsoft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Active Directory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Active Directory, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Active Directory
provider_slug: active-directory
slug: active-directory-domain-security
source_filename: active-directory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 02:11:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: graph.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/active-directory/refs/heads/main/security/active-directory-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Active Directory
- Authentication
- Authorization
- Directory Services
- Identity Management
- Microsoft Entra
- Zero Trust
---
