---
api_specs:
- filename: linearb-openapi.yml
  format: yaml
  label: LinearB Deployments API
  slug: linearb-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linearb/refs/heads/main/openapi/linearb-openapi.yml
- filename: linearb-openapi.yml
  format: yaml
  label: LinearB Incidents API
  slug: linearb-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linearb/refs/heads/main/openapi/linearb-openapi.yml
- filename: linearb-openapi.yml
  format: yaml
  label: LinearB Measurements API
  slug: linearb-measurements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linearb/refs/heads/main/openapi/linearb-openapi.yml
- filename: linearb-openapi.yml
  format: yaml
  label: LinearB Teams API
  slug: linearb-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linearb/refs/heads/main/openapi/linearb-openapi.yml
- filename: linearb-openapi.yml
  format: yaml
  label: LinearB Services API
  slug: linearb-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linearb/refs/heads/main/openapi/linearb-openapi.yml
- filename: linearb-openapi.yml
  format: yaml
  label: LinearB Webhooks API
  slug: linearb-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linearb/refs/heads/main/openapi/linearb-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: linearb.io
  spf: true
hosts:
- cert_expires: Sep 19 09:31:34 2026 GMT
  host: linearb.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 20:03:19 2026 GMT
  host: docs.linearb.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: public-api.linearb.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Linearb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LinearB, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LinearB
provider_slug: linearb
slug: linearb-domain-security
source_filename: linearb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: linearb.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 09:31:34 2026 GMT\n  hsts: null\n- host: docs.linearb.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 20:03:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: public-api.linearb.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: linearb.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linearb/refs/heads/main/security/linearb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Engineering Analytics
- SEI
- Developer Productivity
- DORA Metrics
- DevOps
---
