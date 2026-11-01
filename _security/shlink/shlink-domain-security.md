---
api_specs:
- filename: shlink-domains-api-openapi.yml
  format: yaml
  label: Shlink Domains API
  slug: shlink-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shlink/openapi/shlink-domains-api-openapi.yml
- filename: shlink-integrations-api-openapi.yml
  format: yaml
  label: Shlink Integrations API
  slug: shlink-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shlink/openapi/shlink-integrations-api-openapi.yml
- filename: shlink-monitoring-api-openapi.yml
  format: yaml
  label: Shlink Monitoring API
  slug: shlink-monitoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shlink/openapi/shlink-monitoring-api-openapi.yml
- filename: shlink-redirect-rules-api-openapi.yml
  format: yaml
  label: Shlink Redirect rules API
  slug: shlink-redirect-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shlink/openapi/shlink-redirect-rules-api-openapi.yml
- filename: shlink-short-urls-api-openapi.yml
  format: yaml
  label: Shlink Short URLs API
  slug: shlink-short-urls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shlink/openapi/shlink-short-urls-api-openapi.yml
- filename: shlink-tags-api-openapi.yml
  format: yaml
  label: Shlink Tags API
  slug: shlink-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shlink/openapi/shlink-tags-api-openapi.yml
- filename: shlink-url-shortener-api-openapi.yml
  format: yaml
  label: Shlink URL Shortener API
  slug: shlink-url-shortener-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shlink/openapi/shlink-url-shortener-api-openapi.yml
- filename: shlink-visits-api-openapi.yml
  format: yaml
  label: Shlink Visits API
  slug: shlink-visits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shlink/openapi/shlink-visits-api-openapi.yml
description: ''
domains:
- caa:
  - a5ecwxrv.up.railway.app.
  dmarc: false
  dnssec: true
  domain: shlink.io
  spf: true
hosts:
- cert_expires: Jan 22 11:51:54 2027 GMT
  host: shlink.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Shlink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shlink, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Shlink
provider_slug: shlink
slug: shlink-domain-security
source_filename: shlink-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shlink.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 11:51:54 2027 GMT\n  hsts: false\ndomains:\n- domain: shlink.io\n  dnssec: true\n  caa:\n  - a5ecwxrv.up.railway.app.\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/shlink/security/shlink-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- URL-Shortener
- PHP
- Self-Hosted
- Open-Source
- REST-API
---
