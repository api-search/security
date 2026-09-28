---
api_specs:
- filename: phare-alert-rules-api-openapi.yml
  format: yaml
  label: Phare Alert Rules API
  slug: phare-alert-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phare/refs/heads/main/openapi/phare-alert-rules-api-openapi.yml
- filename: phare-incidents-api-openapi.yml
  format: yaml
  label: Phare Incidents API
  slug: phare-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phare/refs/heads/main/openapi/phare-incidents-api-openapi.yml
- filename: phare-integrations-api-openapi.yml
  format: yaml
  label: Phare Integrations API
  slug: phare-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phare/refs/heads/main/openapi/phare-integrations-api-openapi.yml
- filename: phare-maintenance-windows-api-openapi.yml
  format: yaml
  label: Phare Maintenance Windows API
  slug: phare-maintenance-windows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phare/refs/heads/main/openapi/phare-maintenance-windows-api-openapi.yml
- filename: phare-monitors-api-openapi.yml
  format: yaml
  label: Phare Monitors API
  slug: phare-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phare/refs/heads/main/openapi/phare-monitors-api-openapi.yml
- filename: phare-platform-api-openapi.yml
  format: yaml
  label: Phare Platform API
  slug: phare-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phare/refs/heads/main/openapi/phare-platform-api-openapi.yml
- filename: phare-projects-api-openapi.yml
  format: yaml
  label: Phare Projects API
  slug: phare-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phare/refs/heads/main/openapi/phare-projects-api-openapi.yml
- filename: phare-reports-api-openapi.yml
  format: yaml
  label: Phare Reports API
  slug: phare-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phare/refs/heads/main/openapi/phare-reports-api-openapi.yml
- filename: phare-status-pages-api-openapi.yml
  format: yaml
  label: Phare Status Pages API
  slug: phare-status-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phare/refs/heads/main/openapi/phare-status-pages-api-openapi.yml
- filename: phare-users-api-openapi.yml
  format: yaml
  label: Phare Users API
  slug: phare-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phare/refs/heads/main/openapi/phare-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: phare.io
  spf: true
hosts:
- cert_expires: Nov  3 23:35:23 2026 GMT
  host: phare.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Phare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Phare, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Phare
provider_slug: phare
slug: phare-domain-security
source_filename: phare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: phare.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 23:35:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: phare.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phare/refs/heads/main/security/phare-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Monitoring
- Incident Management
- Analytics
- European
---
