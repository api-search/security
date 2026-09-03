---
api_specs:
- filename: crawlgraph-v1-api-openapi.yml
  format: yaml
  label: CrawlGraph V1 API
  slug: crawlgraph-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crawlgraph/refs/heads/main/openapi/crawlgraph-v1-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: crawlgraph.com
  spf: false
hosts:
- cert_expires: Nov 17 20:31:52 2026 GMT
  host: crawlgraph.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crawlgraph Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CrawlGraph, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: CrawlGraph
provider_slug: crawlgraph
slug: crawlgraph-domain-security
source_filename: crawlgraph-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crawlgraph.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 20:31:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: crawlgraph.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crawlgraph/refs/heads/main/security/crawlgraph-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- SEO
- backlink-intelligence
- MarTech
- Competitive Intelligence
- Web Data
- Common-Crawl
- link-building
- Developer Tools
- MCP
---
