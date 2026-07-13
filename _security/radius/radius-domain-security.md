---
api_specs:
- filename: radius-applications-core-openapi.json
  format: json
  label: Radius Applications.Core API
  slug: applications-core
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radius/refs/heads/main/openapi/radius-applications-core-openapi.json
- filename: radius-applications-dapr-openapi.json
  format: json
  label: Radius Applications.Dapr API
  slug: applications-dapr
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radius/refs/heads/main/openapi/radius-applications-dapr-openapi.json
- filename: radius-applications-datastores-openapi.json
  format: json
  label: Radius Applications.Datastores API
  slug: applications-datastores
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radius/refs/heads/main/openapi/radius-applications-datastores-openapi.json
- filename: radius-applications-messaging-openapi.json
  format: json
  label: Radius Applications.Messaging API
  slug: applications-messaging
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radius/refs/heads/main/openapi/radius-applications-messaging-openapi.json
- filename: radius-ucp-openapi.json
  format: json
  label: Radius Universal Control Plane (UCP) API
  slug: ucp
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radius/refs/heads/main/openapi/radius-ucp-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: radapp.io
  spf: false
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: azure.com
  spf: true
hosts:
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: docs.radapp.io
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 23:36:21 2026 GMT
  host: management.azure.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Radius Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Radius, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Radius
provider_slug: radius
slug: radius-domain-security
source_filename: radius-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.radapp.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 10886400\n- host: management.azure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:36:21 2026 GMT\n  hsts: null\ndomains:\n- domain: radapp.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: azure.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/radius/refs/heads/main/security/radius-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Application Platform
- Cloud Native
- Infrastructure
- Multi Cloud
---
