---
api_specs:
- filename: microsoft-planner-buckets-api-openapi.yml
  format: yaml
  label: Microsoft Planner Buckets API
  slug: microsoft-planner-buckets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-planner/openapi/microsoft-planner-buckets-api-openapi.yml
- filename: microsoft-planner-plan-details-api-openapi.yml
  format: yaml
  label: Microsoft Planner Plan Details API
  slug: microsoft-planner-plan-details-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-planner/openapi/microsoft-planner-plan-details-api-openapi.yml
- filename: microsoft-planner-plans-api-openapi.yml
  format: yaml
  label: Microsoft Planner Plans API
  slug: microsoft-planner-plans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-planner/openapi/microsoft-planner-plans-api-openapi.yml
- filename: microsoft-planner-task-details-api-openapi.yml
  format: yaml
  label: Microsoft Planner Task Details API
  slug: microsoft-planner-task-details-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-planner/openapi/microsoft-planner-task-details-api-openapi.yml
- filename: microsoft-planner-tasks-api-openapi.yml
  format: yaml
  label: Microsoft Planner Tasks API
  slug: microsoft-planner-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-planner/openapi/microsoft-planner-tasks-api-openapi.yml
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
- cert_expires: Jan 17 19:55:21 2027 GMT
  host: www.microsoft.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: May  7 19:07:52 2027 GMT
  host: developer.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  8 00:23:13 2027 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Microsoft Planner Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Planner, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Planner
provider_slug: microsoft-planner
slug: microsoft-planner-domain-security
source_filename: microsoft-planner-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 19:55:21 2027 GMT\n  hsts: false\n- host: developer.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May  7 19:07:52 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  8 00:23:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/microsoft-planner/security/microsoft-planner-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Collaboration
- Microsoft 365
- Productivity
- Project Management
- Task Management
---
