---
api_specs:
- filename: rootly-alerts-api-openapi.yml
  format: yaml
  label: Rootly Alerts API
  slug: rootly-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rootly/refs/heads/main/openapi/rootly-alerts-api-openapi.yml
- filename: rootly-escalation-policies-api-openapi.yml
  format: yaml
  label: Rootly Escalation Policies API
  slug: rootly-escalation-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rootly/refs/heads/main/openapi/rootly-escalation-policies-api-openapi.yml
- filename: rootly-incidents-api-openapi.yml
  format: yaml
  label: Rootly Incidents API
  slug: rootly-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rootly/refs/heads/main/openapi/rootly-incidents-api-openapi.yml
- filename: rootly-services-api-openapi.yml
  format: yaml
  label: Rootly Services API
  slug: rootly-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rootly/refs/heads/main/openapi/rootly-services-api-openapi.yml
- filename: rootly-teams-api-openapi.yml
  format: yaml
  label: Rootly Teams API
  slug: rootly-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rootly/refs/heads/main/openapi/rootly-teams-api-openapi.yml
- filename: rootly-users-api-openapi.yml
  format: yaml
  label: Rootly Users API
  slug: rootly-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rootly/refs/heads/main/openapi/rootly-users-api-openapi.yml
- filename: rootly-workflows-api-openapi.yml
  format: yaml
  label: Rootly Workflows API
  slug: rootly-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rootly/refs/heads/main/openapi/rootly-workflows-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: rootly.com
  spf: true
hosts:
- cert_expires: Oct  6 04:43:31 2026 GMT
  host: rootly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 07:35:16 2026 GMT
  host: api.rootly.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rootly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rootly, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Rootly
provider_slug: rootly
slug: rootly-domain-security
source_filename: rootly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rootly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 04:43:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.rootly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 07:35:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: rootly.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rootly/refs/heads/main/security/rootly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AIOps
- Incident Management
---
