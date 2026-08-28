---
api_specs:
- filename: sana-labs-assignments-api-openapi.yml
  format: yaml
  label: Sana Assignments API
  slug: sana-labs-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana-labs/refs/heads/main/openapi/sana-labs-assignments-api-openapi.yml
- filename: sana-labs-authentication-api-openapi.yml
  format: yaml
  label: Sana Authentication API
  slug: sana-labs-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana-labs/refs/heads/main/openapi/sana-labs-authentication-api-openapi.yml
- filename: sana-labs-courses-api-openapi.yml
  format: yaml
  label: Sana Courses API
  slug: sana-labs-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana-labs/refs/heads/main/openapi/sana-labs-courses-api-openapi.yml
- filename: sana-labs-groups-api-openapi.yml
  format: yaml
  label: Sana Groups API
  slug: sana-labs-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana-labs/refs/heads/main/openapi/sana-labs-groups-api-openapi.yml
- filename: sana-labs-insights-api-openapi.yml
  format: yaml
  label: Sana Insights API
  slug: sana-labs-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana-labs/refs/heads/main/openapi/sana-labs-insights-api-openapi.yml
- filename: sana-labs-paths-api-openapi.yml
  format: yaml
  label: Sana Paths API
  slug: sana-labs-paths-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana-labs/refs/heads/main/openapi/sana-labs-paths-api-openapi.yml
- filename: sana-labs-programs-api-openapi.yml
  format: yaml
  label: Sana Programs API
  slug: sana-labs-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana-labs/refs/heads/main/openapi/sana-labs-programs-api-openapi.yml
- filename: sana-labs-reporting-api-openapi.yml
  format: yaml
  label: Sana Reporting API
  slug: sana-labs-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana-labs/refs/heads/main/openapi/sana-labs-reporting-api-openapi.yml
- filename: sana-labs-teamspaces-api-openapi.yml
  format: yaml
  label: Sana Teamspaces API
  slug: sana-labs-teamspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana-labs/refs/heads/main/openapi/sana-labs-teamspaces-api-openapi.yml
- filename: sana-labs-users-api-openapi.yml
  format: yaml
  label: Sana Users API
  slug: sana-labs-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana-labs/refs/heads/main/openapi/sana-labs-users-api-openapi.yml
- filename: sana-labs-xapi-api-openapi.yml
  format: yaml
  label: Sana xAPI API
  slug: sana-labs-xapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana-labs/refs/heads/main/openapi/sana-labs-xapi-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sana.ai
  spf: true
hosts:
- cert_expires: Aug 20 10:25:05 2026 GMT
  host: www.sana.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 08:49:35 2026 GMT
  host: docs.sana.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: <domain>.sana.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Sana Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sana, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sana
provider_slug: sana-labs
slug: sana-labs-domain-security
source_filename: sana-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sana.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 10:25:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.sana.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 08:49:35 2026 GMT\n  hsts: null\n- host: <domain>.sana.ai\n  https: false\ndomains:\n- domain: sana.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sana-labs/refs/heads/main/security/sana-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Knowledge
- Learning
- LMS
- Agents
- Sweden
---
