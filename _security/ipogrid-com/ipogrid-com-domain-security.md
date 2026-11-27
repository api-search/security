---
api_specs:
- filename: ipogrid-com-articles-api-openapi.yml
  format: yaml
  label: IPOGrid Articles API
  slug: ipogrid-com-articles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ipogrid-com/openapi/ipogrid-com-articles-api-openapi.yml
- filename: ipogrid-com-companies-api-openapi.yml
  format: yaml
  label: IPOGrid Companies API
  slug: ipogrid-com-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ipogrid-com/openapi/ipogrid-com-companies-api-openapi.yml
- filename: ipogrid-com-filings-api-openapi.yml
  format: yaml
  label: IPOGrid Filings API
  slug: ipogrid-com-filings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ipogrid-com/openapi/ipogrid-com-filings-api-openapi.yml
- filename: ipogrid-com-news-api-openapi.yml
  format: yaml
  label: IPOGrid News API
  slug: ipogrid-com-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ipogrid-com/openapi/ipogrid-com-news-api-openapi.yml
- filename: ipogrid-com-outcomes-api-openapi.yml
  format: yaml
  label: IPOGrid Outcomes API
  slug: ipogrid-com-outcomes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ipogrid-com/openapi/ipogrid-com-outcomes-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ipogrid.com
  spf: true
hosts:
- cert_expires: Dec 18 08:45:56 2026 GMT
  host: ipogrid.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: IPOGrid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IPOGrid, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: IPOGrid
provider_slug: ipogrid-com
slug: ipogrid-com-domain-security
source_filename: ipogrid-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ipogrid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 08:45:56 2026 GMT\n  hsts: false\ndomains:\n- domain: ipogrid.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/ipogrid-com/security/ipogrid-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Finance
- IPO
- Data
- Research
- Markets
---
