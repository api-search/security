---
api_specs:
- filename: microsoft-project-assignments-api-openapi.yml
  format: yaml
  label: Microsoft Project Assignments API
  slug: microsoft-project-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/openapi/microsoft-project-assignments-api-openapi.yml
- filename: microsoft-project-calendars-api-openapi.yml
  format: yaml
  label: Microsoft Project Calendars API
  slug: microsoft-project-calendars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/openapi/microsoft-project-calendars-api-openapi.yml
- filename: microsoft-project-custom-fields-api-openapi.yml
  format: yaml
  label: Microsoft Project Custom Fields API
  slug: microsoft-project-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/openapi/microsoft-project-custom-fields-api-openapi.yml
- filename: microsoft-project-enterprise-project-types-api-openapi.yml
  format: yaml
  label: Microsoft Project Enterprise Project Types API
  slug: microsoft-project-enterprise-project-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/openapi/microsoft-project-enterprise-project-types-api-openapi.yml
- filename: microsoft-project-event-handlers-api-openapi.yml
  format: yaml
  label: Microsoft Project Event Handlers API
  slug: microsoft-project-event-handlers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/openapi/microsoft-project-event-handlers-api-openapi.yml
- filename: microsoft-project-lookup-tables-api-openapi.yml
  format: yaml
  label: Microsoft Project Lookup Tables API
  slug: microsoft-project-lookup-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/openapi/microsoft-project-lookup-tables-api-openapi.yml
- filename: microsoft-project-phases-api-openapi.yml
  format: yaml
  label: Microsoft Project Phases API
  slug: microsoft-project-phases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/openapi/microsoft-project-phases-api-openapi.yml
- filename: microsoft-project-projects-api-openapi.yml
  format: yaml
  label: Microsoft Project Projects API
  slug: microsoft-project-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/openapi/microsoft-project-projects-api-openapi.yml
- filename: microsoft-project-resources-api-openapi.yml
  format: yaml
  label: Microsoft Project Resources API
  slug: microsoft-project-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/openapi/microsoft-project-resources-api-openapi.yml
- filename: microsoft-project-stages-api-openapi.yml
  format: yaml
  label: Microsoft Project Stages API
  slug: microsoft-project-stages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/openapi/microsoft-project-stages-api-openapi.yml
- filename: microsoft-project-tasks-api-openapi.yml
  format: yaml
  label: Microsoft Project Tasks API
  slug: microsoft-project-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/openapi/microsoft-project-tasks-api-openapi.yml
- filename: microsoft-project-timesheets-api-openapi.yml
  format: yaml
  label: Microsoft Project Timesheets API
  slug: microsoft-project-timesheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/openapi/microsoft-project-timesheets-api-openapi.yml
- filename: microsoft-project-workflow-activities-api-openapi.yml
  format: yaml
  label: Microsoft Project Workflow Activities API
  slug: microsoft-project-workflow-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/openapi/microsoft-project-workflow-activities-api-openapi.yml
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
- cert_expires: Jan  5 13:03:52 2027 GMT
  host: appsforoffice.microsoft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microsoft Project Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Project, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Project
provider_slug: microsoft-project
slug: microsoft-project-domain-security
source_filename: microsoft-project-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 02:11:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: appsforoffice.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 13:03:52 2027 GMT\n  hsts: null\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/security/microsoft-project-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Budgeting
- Gantt Charts
- Microsoft
- Portfolio Management
- Project Management
- Resource Management
- Scheduling
- Task Management
---
