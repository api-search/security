---
api_specs:
- filename: serpapi-openapi.yml
  format: yaml
  label: SerpApi Bing API
  slug: serpapi-bing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serpapi/refs/heads/main/openapi/serpapi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: serpapi.com
  spf: true
hosts:
- cert_expires: Sep  2 18:14:33 2026 GMT
  host: serpapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Serpapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SerpApi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: SerpApi
provider_slug: serpapi
slug: serpapi-domain-security
source_filename: serpapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: serpapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 18:14:33 2026 GMT\n  hsts: false\ndomains:\n- domain: serpapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/serpapi/refs/heads/main/security/serpapi-domain-security.yml
summary_line: TLSv1.3
tags:
- Bing
- Google
- Search
- Search Engines
---
