---
api_specs:
- filename: microsoft-active-directory-applications-api-openapi.yml
  format: yaml
  label: Microsoft Active Directory Applications API
  slug: microsoft-active-directory-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-active-directory/refs/heads/main/openapi/microsoft-active-directory-applications-api-openapi.yml
- filename: microsoft-active-directory-directory-roles-api-openapi.yml
  format: yaml
  label: Microsoft Active Directory Directory Roles API
  slug: microsoft-active-directory-directory-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-active-directory/refs/heads/main/openapi/microsoft-active-directory-directory-roles-api-openapi.yml
- filename: microsoft-active-directory-groups-api-openapi.yml
  format: yaml
  label: Microsoft Active Directory Groups API
  slug: microsoft-active-directory-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-active-directory/refs/heads/main/openapi/microsoft-active-directory-groups-api-openapi.yml
- filename: microsoft-active-directory-service-principals-api-openapi.yml
  format: yaml
  label: Microsoft Active Directory Service Principals API
  slug: microsoft-active-directory-service-principals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-active-directory/refs/heads/main/openapi/microsoft-active-directory-service-principals-api-openapi.yml
- filename: microsoft-active-directory-users-api-openapi.yml
  format: yaml
  label: Microsoft Active Directory Users API
  slug: microsoft-active-directory-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-active-directory/refs/heads/main/openapi/microsoft-active-directory-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: windows.net
  spf: true
hosts:
- cert_expires: Dec 10 06:59:10 2026 GMT
  host: docs.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 03:53:00 2026 GMT
  host: graph.microsoft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: graph.windows.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microsoft Active Directory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Active Directory, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Active Directory
provider_slug: microsoft-active-directory
slug: microsoft-active-directory-domain-security
source_filename: microsoft-active-directory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 06:59:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: graph.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 03:53:00 2026 GMT\n  hsts: null\n- host: graph.windows.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: windows.net\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-active-directory/refs/heads/main/security/microsoft-active-directory-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Authentication
- Authorization
- Directory Services
- Enterprise
- Identity
- Ldap
- Windows
---
