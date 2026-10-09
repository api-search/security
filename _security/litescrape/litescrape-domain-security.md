---
api_specs:
- filename: litescrape-apple-api-openapi.yml
  format: yaml
  label: Litescrape Apple API
  slug: litescrape-apple-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litescrape/refs/heads/main/openapi/litescrape-apple-api-openapi.yml
- filename: litescrape-bing-api-openapi.yml
  format: yaml
  label: Litescrape Bing API
  slug: litescrape-bing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litescrape/refs/heads/main/openapi/litescrape-bing-api-openapi.yml
- filename: litescrape-duckduckgo-api-openapi.yml
  format: yaml
  label: Litescrape Duckduckgo API
  slug: litescrape-duckduckgo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litescrape/refs/heads/main/openapi/litescrape-duckduckgo-api-openapi.yml
- filename: litescrape-google-api-openapi.yml
  format: yaml
  label: Litescrape Google API
  slug: litescrape-google-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litescrape/refs/heads/main/openapi/litescrape-google-api-openapi.yml
- filename: litescrape-tripadvisor-api-openapi.yml
  format: yaml
  label: Litescrape Tripadvisor API
  slug: litescrape-tripadvisor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litescrape/refs/heads/main/openapi/litescrape-tripadvisor-api-openapi.yml
- filename: litescrape-yelp-api-openapi.yml
  format: yaml
  label: Litescrape Yelp API
  slug: litescrape-yelp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litescrape/refs/heads/main/openapi/litescrape-yelp-api-openapi.yml
- filename: litescrape-zeroclick-api-openapi.yml
  format: yaml
  label: Litescrape Zeroclick API
  slug: litescrape-zeroclick-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litescrape/refs/heads/main/openapi/litescrape-zeroclick-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: litescrape.com
  spf: true
hosts:
- cert_expires: Dec 28 22:34:39 2026 GMT
  host: litescrape.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Litescrape Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Litescrape, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Litescrape
provider_slug: litescrape
slug: litescrape-domain-security
source_filename: litescrape-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: litescrape.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 22:34:39 2026 GMT\n  hsts: null\ndomains:\n- domain: litescrape.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/litescrape/refs/heads/main/security/litescrape-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- SERP API
- Web Scraping
- Search
- Google Maps
- Reviews
- Web Data
- MCP
---
