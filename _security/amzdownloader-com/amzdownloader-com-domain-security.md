---
api_specs:
- filename: amzdownloader-com-account-api-openapi.yml
  format: yaml
  label: AMZ Downloader Account API
  slug: amzdownloader-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amzdownloader-com/openapi/amzdownloader-com-account-api-openapi.yml
- filename: amzdownloader-com-discovery-api-openapi.yml
  format: yaml
  label: AMZ Downloader Discovery API
  slug: amzdownloader-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amzdownloader-com/openapi/amzdownloader-com-discovery-api-openapi.yml
- filename: amzdownloader-com-extraction-api-openapi.yml
  format: yaml
  label: AMZ Downloader Extraction API
  slug: amzdownloader-com-extraction-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amzdownloader-com/openapi/amzdownloader-com-extraction-api-openapi.yml
- filename: amzdownloader-com-media-api-openapi.yml
  format: yaml
  label: AMZ Downloader Media API
  slug: amzdownloader-com-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amzdownloader-com/openapi/amzdownloader-com-media-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: amzdownloader.com
  spf: true
hosts:
- cert_expires: Jan 17 08:47:05 2027 GMT
  host: amzdownloader.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AMZ Downloader Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AMZ Downloader, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AMZ Downloader
provider_slug: amzdownloader-com
slug: amzdownloader-com-domain-security
source_filename: amzdownloader-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: amzdownloader.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 08:47:05 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: amzdownloader.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/amzdownloader-com/security/amzdownloader-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Media
- Amazon
- Downloader
---
