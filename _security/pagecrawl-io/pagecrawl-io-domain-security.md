---
api_specs:
- filename: pagecrawl-io-openapi-generated.yml
  format: yaml
  label: PageCrawl.io API
  slug: pagecrawl-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagecrawl-io/openapi/_ae-authored/pagecrawl-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: pagecrawl.io
  spf: true
hosts:
- cert_expires: Feb  5 11:15:30 2027 GMT
  host: pagecrawl.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: PageCrawl.io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PageCrawl.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: PageCrawl.io
provider_slug: pagecrawl-io
slug: pagecrawl-io-domain-security
source_filename: pagecrawl-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pagecrawl.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 11:15:30 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pagecrawl.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/pagecrawl-io/security/pagecrawl-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Monitoring
- Artificial Intelligence
- Change Detection
- Software-as-a-Service
---
