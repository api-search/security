---
api_specs:
- filename: rss-openapi.yml
  format: yaml
  label: The Philadelphia Inquirer RSS Feeds
  slug: rss
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/philadelphia-inquirer/refs/heads/main/openapi/rss-openapi.yml
- filename: sitemaps-openapi.yml
  format: yaml
  label: The Philadelphia Inquirer Sitemaps
  slug: sitemaps
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/philadelphia-inquirer/refs/heads/main/openapi/sitemaps-openapi.yml
- filename: dewey-mcp-openapi.yml
  format: yaml
  label: Dewey MCP
  slug: dewey-mcp
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/philadelphia-inquirer/refs/heads/main/openapi/dewey-mcp-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: inquirer.com
  spf: true
hosts:
- cert_expires: Sep 24 06:40:28 2026 GMT
  host: www.inquirer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: 127.0.0.1
  https: false
kind: domain-security
layout: security
method: probed
name: Philadelphia Inquirer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Philadelphia Inquirer, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: The Philadelphia Inquirer
provider_slug: philadelphia-inquirer
slug: philadelphia-inquirer-domain-security
source_filename: philadelphia-inquirer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.inquirer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 06:40:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: 127.0.0.1\n  https: false\ndomains:\n- domain: inquirer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/philadelphia-inquirer/refs/heads/main/security/philadelphia-inquirer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- News
- News Media
- Newspaper
- Journalism
- Philadelphia
- Pennsylvania
- Local News
- RSS
- Sitemap
- Arc Publishing
- MCP
---
