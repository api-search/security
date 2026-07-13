---
api_specs:
- filename: visio-javascript-openapi.yml
  format: yaml
  label: Visio JavaScript API
  slug: visio-javascript-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visio/refs/heads/main/openapi/visio-javascript-openapi.yml
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
- cert_expires: Jan  5 13:03:52 2027 GMT
  host: appsforoffice.microsoft.com
  hsts: null
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
name: Visio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Visio API, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Visio API
provider_slug: visio
slug: visio-domain-security
source_filename: visio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: appsforoffice.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 13:03:52 2027 GMT\n  hsts: null\n- host: graph.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 03:53:00 2026 GMT\n  hsts: null\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/visio/refs/heads/main/security/visio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Business Process
- Collaboration
- Diagrams
- Enterprise
- Flowcharts
- Microsoft 365
- Visualization
---
