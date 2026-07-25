---
api_specs:
- filename: microsoft-office-365-calendar-api-openapi.yml
  format: yaml
  label: Microsoft Office 365 Calendar API
  slug: microsoft-office-365-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-365/refs/heads/main/openapi/microsoft-office-365-calendar-api-openapi.yml
- filename: microsoft-office-365-groups-api-openapi.yml
  format: yaml
  label: Microsoft Office 365 Groups API
  slug: microsoft-office-365-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-365/refs/heads/main/openapi/microsoft-office-365-groups-api-openapi.yml
- filename: microsoft-office-365-mail-api-openapi.yml
  format: yaml
  label: Microsoft Office 365 Mail API
  slug: microsoft-office-365-mail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-365/refs/heads/main/openapi/microsoft-office-365-mail-api-openapi.yml
- filename: microsoft-office-365-users-api-openapi.yml
  format: yaml
  label: Microsoft Office 365 Users API
  slug: microsoft-office-365-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-365/refs/heads/main/openapi/microsoft-office-365-users-api-openapi.yml
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
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: graph.microsoft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 06:59:10 2026 GMT
  host: docs.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microsoft Office 365 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Office 365, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Office 365
provider_slug: microsoft-office-365
slug: microsoft-office-365-domain-security
source_filename: microsoft-office-365-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 02:11:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: graph.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: null\n- host: docs.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 06:59:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-365/refs/heads/main/security/microsoft-office-365-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud
- Collaboration
- Enterprise
- Microsoft
- Productivity
---
