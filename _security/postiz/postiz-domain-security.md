---
api_specs:
- filename: postiz-analytics-api-openapi.yml
  format: yaml
  label: Postiz Analytics API
  slug: postiz-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postiz/refs/heads/main/openapi/postiz-analytics-api-openapi.yml
- filename: postiz-integrations-api-openapi.yml
  format: yaml
  label: Postiz Integrations API
  slug: postiz-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postiz/refs/heads/main/openapi/postiz-integrations-api-openapi.yml
- filename: postiz-notifications-api-openapi.yml
  format: yaml
  label: Postiz Notifications API
  slug: postiz-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postiz/refs/heads/main/openapi/postiz-notifications-api-openapi.yml
- filename: postiz-posts-api-openapi.yml
  format: yaml
  label: Postiz Posts API
  slug: postiz-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postiz/refs/heads/main/openapi/postiz-posts-api-openapi.yml
- filename: postiz-uploads-api-openapi.yml
  format: yaml
  label: Postiz Uploads API
  slug: postiz-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postiz/refs/heads/main/openapi/postiz-uploads-api-openapi.yml
- filename: postiz-public-api-openapi.json
  format: json
  label: Postiz Public API
  slug: postiz-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postiz/refs/heads/main/openapi/postiz-public-api-openapi.json
- filename: postiz-platform-swagger-openapi.json
  format: json
  label: Postiz Platform API
  slug: postiz-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postiz/refs/heads/main/openapi/postiz-platform-swagger-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: postiz.com
  spf: true
hosts:
- cert_expires: Sep 23 15:48:44 2026 GMT
  host: postiz.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 19:18:34 2026 GMT
  host: docs.postiz.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 07:28:49 2026 GMT
  host: api.postiz.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Postiz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Postiz, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Postiz
provider_slug: postiz
slug: postiz-domain-security
source_filename: postiz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: postiz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 15:48:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.postiz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 19:18:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.postiz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 07:28:49 2026 GMT\n  hsts: false\ndomains:\n- domain: postiz.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/postiz/refs/heads/main/security/postiz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Social-Media
- Scheduling
- Open-Source
- Content
- Marketing
- Agents
- MCP
- Automation
- Publishing
- Analytics
---
