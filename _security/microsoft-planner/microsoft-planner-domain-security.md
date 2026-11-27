---
api_specs:
- filename: microsoft-planner-groups-plannergroup-api-openapi.yml
  format: yaml
  label: Microsoft Planner Groups.planner Group API
  slug: microsoft-planner-groups-plannergroup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-planner/openapi/microsoft-planner-groups-plannergroup-api-openapi.yml
- filename: microsoft-planner-me-planneruser-api-openapi.yml
  format: yaml
  label: Microsoft Planner Me.planner User API
  slug: microsoft-planner-me-planneruser-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-planner/openapi/microsoft-planner-me-planneruser-api-openapi.yml
- filename: microsoft-planner-planner-planner-api-openapi.yml
  format: yaml
  label: Microsoft Planner Planner.planner API
  slug: microsoft-planner-planner-planner-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-planner/openapi/microsoft-planner-planner-planner-api-openapi.yml
- filename: microsoft-planner-planner-plannerbucket-api-openapi.yml
  format: yaml
  label: Microsoft Planner Planner.planner Bucket API
  slug: microsoft-planner-planner-plannerbucket-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-planner/openapi/microsoft-planner-planner-plannerbucket-api-openapi.yml
- filename: microsoft-planner-planner-plannerplan-api-openapi.yml
  format: yaml
  label: Microsoft Planner Planner.planner Plan API
  slug: microsoft-planner-planner-plannerplan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-planner/openapi/microsoft-planner-planner-plannerplan-api-openapi.yml
- filename: microsoft-planner-planner-plannertask-api-openapi.yml
  format: yaml
  label: Microsoft Planner Planner.planner Task API
  slug: microsoft-planner-planner-plannertask-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-planner/openapi/microsoft-planner-planner-plannertask-api-openapi.yml
- filename: microsoft-planner-users-planneruser-api-openapi.yml
  format: yaml
  label: Microsoft Planner Users.planner User API
  slug: microsoft-planner-users-planneruser-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-planner/openapi/microsoft-planner-users-planneruser-api-openapi.yml
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
  hsts: null
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
overview: 'Domain security posture for Microsoft Planner, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Planner
provider_slug: microsoft-planner
slug: microsoft-planner-domain-security
source_filename: microsoft-planner-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 19:55:21 2027 GMT\n  hsts: false\n- host: developer.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May  7 19:07:52 2027 GMT\n  hsts: null\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  8 00:23:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/microsoft-planner/security/microsoft-planner-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Collaboration
- Microsoft 365
- Productivity
- Project Management
- Task Management
---
