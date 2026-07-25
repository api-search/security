---
api_specs:
- filename: sana-assignments-api-openapi.yml
  format: yaml
  label: Sana Assignments API
  slug: sana-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana/refs/heads/main/openapi/sana-assignments-api-openapi.yml
- filename: sana-authentication-api-openapi.yml
  format: yaml
  label: Sana Authentication API
  slug: sana-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana/refs/heads/main/openapi/sana-authentication-api-openapi.yml
- filename: sana-courses-api-openapi.yml
  format: yaml
  label: Sana Courses API
  slug: sana-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana/refs/heads/main/openapi/sana-courses-api-openapi.yml
- filename: sana-groups-api-openapi.yml
  format: yaml
  label: Sana Groups API
  slug: sana-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana/refs/heads/main/openapi/sana-groups-api-openapi.yml
- filename: sana-paths-api-openapi.yml
  format: yaml
  label: Sana Paths API
  slug: sana-paths-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana/refs/heads/main/openapi/sana-paths-api-openapi.yml
- filename: sana-programs-api-openapi.yml
  format: yaml
  label: Sana Programs API
  slug: sana-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana/refs/heads/main/openapi/sana-programs-api-openapi.yml
- filename: sana-reporting-api-openapi.yml
  format: yaml
  label: Sana Reporting API
  slug: sana-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana/refs/heads/main/openapi/sana-reporting-api-openapi.yml
- filename: sana-teamspaces-api-openapi.yml
  format: yaml
  label: Sana Teamspaces API
  slug: sana-teamspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana/refs/heads/main/openapi/sana-teamspaces-api-openapi.yml
- filename: sana-users-api-openapi.yml
  format: yaml
  label: Sana Users API
  slug: sana-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana/refs/heads/main/openapi/sana-users-api-openapi.yml
- filename: sana-xapi-api-openapi.yml
  format: yaml
  label: Sana xAPI API
  slug: sana-xapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana/refs/heads/main/openapi/sana-xapi-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sanalabs.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sana.ai
  spf: true
hosts:
- cert_expires: Sep 16 04:13:46 2026 GMT
  host: www.sanalabs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 08:49:35 2026 GMT
  host: docs.sana.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 08:49:35 2026 GMT
  host: app.sana.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sana Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sana, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sana
provider_slug: sana
slug: sana-domain-security
source_filename: sana-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sanalabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 04:13:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.sana.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 08:49:35 2026 GMT\n  hsts: null\n- host: app.sana.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 08:49:35 2026 GMT\n  hsts: null\ndomains:\n- domain: sanalabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: sana.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sana/refs/heads/main/security/sana-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise AI
- Artificial Intelligence
- Learning Management
- LMS
- Knowledge Management
- Agents
- SCIM
- xAPI
- REST API
---
