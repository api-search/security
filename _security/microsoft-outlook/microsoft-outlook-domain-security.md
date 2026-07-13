---
api_specs:
- filename: microsoft-graph-mail-api-openapi.yml
  format: yaml
  label: Microsoft Graph Mail API
  slug: microsoft-graph-mail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-outlook/refs/heads/main/openapi/microsoft-graph-mail-api-openapi.yml
- filename: openapi.yaml
  format: yaml
  label: Microsoft Graph Calendar API
  slug: microsoft-graph-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/msgraph-metadata/master/openapi/v1.0/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Microsoft Graph Contacts API
  slug: microsoft-graph-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/msgraph-metadata/master/openapi/v1.0/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Microsoft Graph Tasks API
  slug: microsoft-graph-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/msgraph-metadata/master/openapi/v1.0/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Microsoft Graph People API
  slug: microsoft-graph-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/msgraph-metadata/master/openapi/v1.0/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Microsoft Graph Change Notifications API
  slug: microsoft-graph-change-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/msgraph-metadata/master/openapi/v1.0/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Microsoft Graph Focused Inbox API
  slug: microsoft-graph-focused-inbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/msgraph-metadata/master/openapi/v1.0/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Microsoft Graph Mail Rules API
  slug: microsoft-graph-mail-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/msgraph-metadata/master/openapi/v1.0/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Microsoft Graph Categories API
  slug: microsoft-graph-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/msgraph-metadata/master/openapi/v1.0/openapi.yaml
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
- cert_expires: Dec  2 03:53:00 2026 GMT
  host: graph.microsoft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microsoft Outlook Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Outlook, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Outlook
provider_slug: microsoft-outlook
slug: microsoft-outlook-domain-security
source_filename: microsoft-outlook-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 02:11:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: graph.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 03:53:00 2026 GMT\n  hsts: null\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-outlook/refs/heads/main/security/microsoft-outlook-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Calendar
- Contacts
- Email
- Enterprise
- Microsoft
- Office 365
- Productivity
---
