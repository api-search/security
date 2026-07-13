---
api_specs:
- filename: microsoft-exchange-graph-mail-openapi.yml
  format: yaml
  label: Microsoft Graph Mail API
  slug: microsoft-graph-mail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-graph-mail-openapi.yml
- filename: microsoft-exchange-graph-calendar-openapi.yml
  format: yaml
  label: Microsoft Graph Calendar API
  slug: microsoft-graph-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-graph-calendar-openapi.yml
- filename: microsoft-exchange-graph-contacts-openapi.yml
  format: yaml
  label: Microsoft Graph Contacts API
  slug: microsoft-graph-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-graph-contacts-openapi.yml
- filename: microsoft-exchange-graph-people-openapi.yml
  format: yaml
  label: Microsoft Graph People API
  slug: microsoft-graph-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-graph-people-openapi.yml
- filename: microsoft-exchange-admin-api-openapi.yml
  format: yaml
  label: Exchange Online Admin API
  slug: exchange-online-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-admin-api-openapi.yml
- filename: microsoft-exchange-graph-import-export-openapi.yml
  format: yaml
  label: Microsoft Graph Mailbox Import Export API
  slug: microsoft-graph-mailbox-import-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-graph-import-export-openapi.yml
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
- cert_expires: Jan 17 19:55:21 2027 GMT
  host: www.microsoft.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microsoft Exchange Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Exchange, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Exchange
provider_slug: microsoft-exchange
slug: microsoft-exchange-domain-security
source_filename: microsoft-exchange-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 02:11:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 19:55:21 2027 GMT\n  hsts: false\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/security/microsoft-exchange-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Calendar
- Collaboration
- Contacts
- Email
- Enterprise
---
