---
api_specs:
- filename: edgegap-openapi.yml
  format: yaml
  label: Edgegap Applications API
  slug: edgegap-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgegap/refs/heads/main/openapi/edgegap-openapi.yml
- filename: edgegap-openapi.yml
  format: yaml
  label: Edgegap App Versions API
  slug: edgegap-app-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgegap/refs/heads/main/openapi/edgegap-openapi.yml
- filename: edgegap-openapi.yml
  format: yaml
  label: Edgegap Deployments API
  slug: edgegap-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgegap/refs/heads/main/openapi/edgegap-openapi.yml
- filename: edgegap-openapi.yml
  format: yaml
  label: Edgegap Sessions API
  slug: edgegap-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgegap/refs/heads/main/openapi/edgegap-openapi.yml
- filename: edgegap-openapi.yml
  format: yaml
  label: Edgegap Matchmaking API
  slug: edgegap-matchmaking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgegap/refs/heads/main/openapi/edgegap-openapi.yml
- filename: edgegap-openapi.yml
  format: yaml
  label: Edgegap Relays API
  slug: edgegap-relays-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgegap/refs/heads/main/openapi/edgegap-openapi.yml
- filename: edgegap-openapi.yml
  format: yaml
  label: Edgegap Metrics API
  slug: edgegap-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgegap/refs/heads/main/openapi/edgegap-openapi.yml
- filename: edgegap-openapi.yml
  format: yaml
  label: Edgegap Fleets API
  slug: edgegap-fleets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgegap/refs/heads/main/openapi/edgegap-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: edgegap.com
  spf: true
hosts:
- cert_expires: Sep 28 23:59:59 2026 GMT
  host: edgegap.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 23:13:51 2026 GMT
  host: docs.edgegap.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 02:40:52 2026 GMT
  host: api.edgegap.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Edgegap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Edgegap, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Edgegap
provider_slug: edgegap
slug: edgegap-domain-security
source_filename: edgegap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: edgegap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.edgegap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:13:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.edgegap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 02:40:52 2026 GMT\n  hsts: null\ndomains:\n- domain: edgegap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edgegap/refs/heads/main/security/edgegap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Game Servers
- Orchestration
- Edge Computing
- Matchmaking
- Hosting
---
