---
api_specs:
- filename: crawlora-net-openapi-generated.yml
  format: yaml
  label: crawlora-net API
  slug: crawlora-net-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crawlora-net/openapi/_ae-authored/crawlora-net-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: crawlora.net
  spf: true
hosts:
- cert_expires: Dec  1 16:32:54 2026 GMT
  host: crawlora.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Crawlora Net Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for crawlora-net, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: crawlora-net
provider_slug: crawlora-net
slug: crawlora-net-domain-security
source_filename: crawlora-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crawlora.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 16:32:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: crawlora.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/crawlora-net/security/crawlora-net-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Web Scraping
- AI
- Data
- MCP
---
