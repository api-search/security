---
api_specs:
- filename: microsoft-exchange-accepted-domains-api-openapi.yml
  format: yaml
  label: Microsoft Exchange Accepted Domains API
  slug: microsoft-exchange-accepted-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-accepted-domains-api-openapi.yml
- filename: microsoft-exchange-attachments-api-openapi.yml
  format: yaml
  label: Microsoft Exchange Attachments API
  slug: microsoft-exchange-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-attachments-api-openapi.yml
- filename: microsoft-exchange-calendars-api-openapi.yml
  format: yaml
  label: Microsoft Exchange Calendars API
  slug: microsoft-exchange-calendars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-calendars-api-openapi.yml
- filename: microsoft-exchange-contact-folders-api-openapi.yml
  format: yaml
  label: Microsoft Exchange Contact Folders API
  slug: microsoft-exchange-contact-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-contact-folders-api-openapi.yml
- filename: microsoft-exchange-contacts-api-openapi.yml
  format: yaml
  label: Microsoft Exchange Contacts API
  slug: microsoft-exchange-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-contacts-api-openapi.yml
- filename: microsoft-exchange-distribution-groups-api-openapi.yml
  format: yaml
  label: Microsoft Exchange Distribution Groups API
  slug: microsoft-exchange-distribution-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-distribution-groups-api-openapi.yml
- filename: microsoft-exchange-events-api-openapi.yml
  format: yaml
  label: Microsoft Exchange Events API
  slug: microsoft-exchange-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-events-api-openapi.yml
- filename: microsoft-exchange-mail-folders-api-openapi.yml
  format: yaml
  label: Microsoft Exchange Mail Folders API
  slug: microsoft-exchange-mail-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-mail-folders-api-openapi.yml
- filename: microsoft-exchange-mailbox-discovery-api-openapi.yml
  format: yaml
  label: Microsoft Exchange Mailbox Discovery API
  slug: microsoft-exchange-mailbox-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-mailbox-discovery-api-openapi.yml
- filename: microsoft-exchange-mailbox-export-api-openapi.yml
  format: yaml
  label: Microsoft Exchange Mailbox Export API
  slug: microsoft-exchange-mailbox-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-mailbox-export-api-openapi.yml
- filename: microsoft-exchange-mailbox-folder-permissions-api-openapi.yml
  format: yaml
  label: Microsoft Exchange Mailbox Folder Permissions API
  slug: microsoft-exchange-mailbox-folder-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-mailbox-folder-permissions-api-openapi.yml
- filename: microsoft-exchange-mailbox-import-api-openapi.yml
  format: yaml
  label: Microsoft Exchange Mailbox Import API
  slug: microsoft-exchange-mailbox-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-mailbox-import-api-openapi.yml
- filename: microsoft-exchange-mailboxes-api-openapi.yml
  format: yaml
  label: Microsoft Exchange Mailboxes API
  slug: microsoft-exchange-mailboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-mailboxes-api-openapi.yml
- filename: microsoft-exchange-messages-api-openapi.yml
  format: yaml
  label: Microsoft Exchange Messages API
  slug: microsoft-exchange-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-messages-api-openapi.yml
- filename: microsoft-exchange-organization-configuration-api-openapi.yml
  format: yaml
  label: Microsoft Exchange Organization Configuration API
  slug: microsoft-exchange-organization-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-organization-configuration-api-openapi.yml
- filename: microsoft-exchange-people-api-openapi.yml
  format: yaml
  label: Microsoft Exchange People API
  slug: microsoft-exchange-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-people-api-openapi.yml
- filename: microsoft-exchange-scheduling-api-openapi.yml
  format: yaml
  label: Microsoft Exchange Scheduling API
  slug: microsoft-exchange-scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/openapi/microsoft-exchange-scheduling-api-openapi.yml
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
