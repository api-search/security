---
api_specs:
- filename: microsoft-to-do-me-todo-api-openapi.yml
  format: yaml
  label: Microsoft To Do Me.todo API
  slug: microsoft-to-do-me-todo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-to-do/openapi/microsoft-to-do-me-todo-api-openapi.yml
- filename: microsoft-to-do-users-todo-api-openapi.yml
  format: yaml
  label: Microsoft To Do Users.todo API
  slug: microsoft-to-do-users-todo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-to-do/openapi/microsoft-to-do-users-todo-api-openapi.yml
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
- cert_expires: Jan 30 15:08:02 2027 GMT
  host: to-do.microsoft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 17 19:55:21 2027 GMT
  host: www.microsoft.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  8 00:23:13 2027 GMT
  host: learn.microsoft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Microsoft To Do Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft To Do, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft To Do
provider_slug: microsoft-to-do
slug: microsoft-to-do-domain-security
source_filename: microsoft-to-do-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: to-do.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 15:08:02 2027 GMT\n  hsts: null\n- host: www.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 19:55:21 2027 GMT\n  hsts: false\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  8 00:23:13 2027 GMT\n  hsts: null\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/microsoft-to-do/security/microsoft-to-do-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Microsoft
- Microsoft 365
- Productivity
- Task
- Task Management
- Microsoft Graph
---
