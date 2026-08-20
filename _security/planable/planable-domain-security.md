---
api_specs:
- filename: planable-campaigns-api-openapi.yml
  format: yaml
  label: Planable Campaigns API
  slug: planable-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planable/refs/heads/main/openapi/planable-campaigns-api-openapi.yml
- filename: planable-competitors-api-openapi.yml
  format: yaml
  label: Planable Competitors API
  slug: planable-competitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planable/refs/heads/main/openapi/planable-competitors-api-openapi.yml
- filename: planable-labels-api-openapi.yml
  format: yaml
  label: Planable Labels API
  slug: planable-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planable/refs/heads/main/openapi/planable-labels-api-openapi.yml
- filename: planable-media-api-openapi.yml
  format: yaml
  label: Planable Media API
  slug: planable-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planable/refs/heads/main/openapi/planable-media-api-openapi.yml
- filename: planable-members-api-openapi.yml
  format: yaml
  label: Planable Members API
  slug: planable-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planable/refs/heads/main/openapi/planable-members-api-openapi.yml
- filename: planable-pages-api-openapi.yml
  format: yaml
  label: Planable Pages API
  slug: planable-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planable/refs/heads/main/openapi/planable-pages-api-openapi.yml
- filename: planable-posts-api-openapi.yml
  format: yaml
  label: Planable Posts API
  slug: planable-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planable/refs/heads/main/openapi/planable-posts-api-openapi.yml
- filename: planable-social-listening-api-openapi.yml
  format: yaml
  label: Planable Social Listening API
  slug: planable-social-listening-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planable/refs/heads/main/openapi/planable-social-listening-api-openapi.yml
- filename: planable-stories-api-openapi.yml
  format: yaml
  label: Planable Stories API
  slug: planable-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planable/refs/heads/main/openapi/planable-stories-api-openapi.yml
- filename: planable-system-api-openapi.yml
  format: yaml
  label: Planable System API
  slug: planable-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planable/refs/heads/main/openapi/planable-system-api-openapi.yml
- filename: planable-workspaces-api-openapi.yml
  format: yaml
  label: Planable Workspaces API
  slug: planable-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planable/refs/heads/main/openapi/planable-workspaces-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: planable.io
  spf: true
hosts:
- cert_expires: Oct 15 15:48:00 2026 GMT
  host: planable.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 02:53:37 2026 GMT
  host: app.planable.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 11:35:56 2026 GMT
  host: api.planable.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Planable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Planable, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Planable
provider_slug: planable
slug: planable-domain-security
source_filename: planable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: planable.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 15:48:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.planable.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 02:53:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.planable.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 11:35:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: planable.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/planable/refs/heads/main/security/planable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Social-Media
- Content Collaboration
- Approval Workflows
- Social Media Management
- Content Publishing
- Marketing
- Social Media Analytics
- Social Listening
- MCP
- AI Agents
- Agent Skills
---
