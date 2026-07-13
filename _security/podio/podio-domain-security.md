---
api_specs:
- filename: podio-openapi.yml
  format: yaml
  label: Podio REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podio/refs/heads/main/openapi/podio-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: podio.com
  spf: true
hosts:
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: www.podio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 29 23:59:59 2026 GMT
  host: developers.podio.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 29 23:59:59 2026 GMT
  host: api.podio.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Podio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Podio, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Podio
provider_slug: podio
slug: podio-domain-security
source_filename: podio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.podio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: false\n- host: developers.podio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.podio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: podio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/podio/refs/heads/main/security/podio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Work Management
- Collaboration
- Project Management
- CRM
- Workflow
- Custom Apps
---
