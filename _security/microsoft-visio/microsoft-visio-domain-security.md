---
api_specs:
- filename: microsoft-visio-comments-api-openapi.yml
  format: yaml
  label: Microsoft Visio Comments API
  slug: microsoft-visio-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-visio/refs/heads/main/openapi/microsoft-visio-comments-api-openapi.yml
- filename: microsoft-visio-documents-api-openapi.yml
  format: yaml
  label: Microsoft Visio Documents API
  slug: microsoft-visio-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-visio/refs/heads/main/openapi/microsoft-visio-documents-api-openapi.yml
- filename: microsoft-visio-hyperlinks-api-openapi.yml
  format: yaml
  label: Microsoft Visio Hyperlinks API
  slug: microsoft-visio-hyperlinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-visio/refs/heads/main/openapi/microsoft-visio-hyperlinks-api-openapi.yml
- filename: microsoft-visio-pages-api-openapi.yml
  format: yaml
  label: Microsoft Visio Pages API
  slug: microsoft-visio-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-visio/refs/heads/main/openapi/microsoft-visio-pages-api-openapi.yml
- filename: microsoft-visio-shape-data-api-openapi.yml
  format: yaml
  label: Microsoft Visio Shape Data API
  slug: microsoft-visio-shape-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-visio/refs/heads/main/openapi/microsoft-visio-shape-data-api-openapi.yml
- filename: microsoft-visio-shapes-api-openapi.yml
  format: yaml
  label: Microsoft Visio Shapes API
  slug: microsoft-visio-shapes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-visio/refs/heads/main/openapi/microsoft-visio-shapes-api-openapi.yml
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
name: Microsoft Visio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Visio, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Visio
provider_slug: microsoft-visio
slug: microsoft-visio-domain-security
source_filename: microsoft-visio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: graph.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 03:53:00 2026 GMT\n  hsts: null\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-visio/refs/heads/main/security/microsoft-visio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Business Process
- Diagramming
- Flowcharts
- Microsoft 365
- Visualization
---
