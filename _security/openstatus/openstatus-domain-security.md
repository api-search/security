---
api_specs:
- filename: openstatus-openapi.yml
  format: yaml
  label: OpenStatus Monitors
  slug: monitors
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstatus/refs/heads/main/openapi/openstatus-openapi.yml
- filename: openstatus-openapi.yml
  format: yaml
  label: OpenStatus Incidents
  slug: incidents
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstatus/refs/heads/main/openapi/openstatus-openapi.yml
- filename: openstatus-openapi.yml
  format: yaml
  label: OpenStatus Status Reports
  slug: status-reports
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstatus/refs/heads/main/openapi/openstatus-openapi.yml
- filename: openstatus-openapi.yml
  format: yaml
  label: OpenStatus Status Pages
  slug: status-pages
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstatus/refs/heads/main/openapi/openstatus-openapi.yml
- filename: openstatus-openapi.yml
  format: yaml
  label: OpenStatus Checks
  slug: checks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstatus/refs/heads/main/openapi/openstatus-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openstatus.dev
  spf: true
hosts:
- cert_expires: Sep 15 21:15:32 2026 GMT
  host: www.openstatus.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 23:24:22 2026 GMT
  host: api.openstatus.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openstatus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenStatus, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OpenStatus
provider_slug: openstatus
slug: openstatus-domain-security
source_filename: openstatus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.openstatus.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 21:15:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.openstatus.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:24:22 2026 GMT\n  hsts: null\ndomains:\n- domain: openstatus.dev\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openstatus/refs/heads/main/security/openstatus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Monitoring
- Synthetic Monitoring
- Uptime
- Status Pages
- Incidents
- Open Source
- Observability
---
