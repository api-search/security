---
api_specs:
- filename: notion-blocks-api-openapi.yml
  format: yaml
  label: Notion Blocks API
  slug: notion-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notion/refs/heads/main/openapi/notion-blocks-api-openapi.yml
- filename: notion-comments-api-openapi.yml
  format: yaml
  label: Notion Comments API
  slug: notion-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notion/refs/heads/main/openapi/notion-comments-api-openapi.yml
- filename: notion-databases-api-openapi.yml
  format: yaml
  label: Notion Databases API
  slug: notion-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notion/refs/heads/main/openapi/notion-databases-api-openapi.yml
- filename: notion-pages-api-openapi.yml
  format: yaml
  label: Notion Pages API
  slug: notion-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notion/refs/heads/main/openapi/notion-pages-api-openapi.yml
- filename: notion-search-api-openapi.yml
  format: yaml
  label: Notion Search API
  slug: notion-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notion/refs/heads/main/openapi/notion-search-api-openapi.yml
- filename: notion-users-api-openapi.yml
  format: yaml
  label: Notion Users API
  slug: notion-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notion/refs/heads/main/openapi/notion-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: notion.so
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: notion.com
  spf: true
hosts:
- cert_expires: Sep 13 23:41:14 2026 GMT
  host: www.notion.so
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 09:55:45 2026 GMT
  host: developers.notion.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 02:58:03 2026 GMT
  host: api.notion.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Notion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Notion, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Notion
provider_slug: notion
slug: notion-domain-security
source_filename: notion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.notion.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:41:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.notion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 09:55:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.notion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 02:58:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: notion.so\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: notion.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/notion/refs/heads/main/security/notion-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Collaboration
- Database
- Ideas
- Notes
- Productivity
- Project
- T1
- Task
- Wiki
- Workspace
---
