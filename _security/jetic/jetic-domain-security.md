---
api_specs:
- filename: jetic-api-specifications-api-openapi.yml
  format: yaml
  label: Jetic API Specifications API
  slug: jetic-api-specifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jetic/refs/heads/main/openapi/jetic-api-specifications-api-openapi.yml
- filename: jetic-clusters-api-openapi.yml
  format: yaml
  label: Jetic Clusters API
  slug: jetic-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jetic/refs/heads/main/openapi/jetic-clusters-api-openapi.yml
- filename: jetic-deployments-api-openapi.yml
  format: yaml
  label: Jetic Deployments API
  slug: jetic-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jetic/refs/heads/main/openapi/jetic-deployments-api-openapi.yml
- filename: jetic-integrations-api-openapi.yml
  format: yaml
  label: Jetic Integrations API
  slug: jetic-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jetic/refs/heads/main/openapi/jetic-integrations-api-openapi.yml
- filename: jetic-monitoring-api-openapi.yml
  format: yaml
  label: Jetic Monitoring API
  slug: jetic-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jetic/refs/heads/main/openapi/jetic-monitoring-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jetic.io
  spf: true
hosts:
- cert_expires: Oct  4 22:03:45 2026 GMT
  host: jetic.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 12:53:41 2026 GMT
  host: docs.jetic.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 08:36:06 2026 GMT
  host: app.us1.jetic.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jetic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jetic, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Jetic
provider_slug: jetic
slug: jetic-domain-security
source_filename: jetic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jetic.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 22:03:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.jetic.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 12:53:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.us1.jetic.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 08:36:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jetic.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jetic/refs/heads/main/security/jetic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Apache Camel
- Integrations
- iPaaS
- Pro-Code API Composition
---
