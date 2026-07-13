---
api_specs:
- filename: starwood-hotel-search-openapi.yml
  format: yaml
  label: Hotel Search API
  slug: hotel-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starwood-hotels-and-resorts/refs/heads/main/openapi/starwood-hotel-search-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: starwoodhotels.com
  spf: true
hosts:
- cert_expires: Sep 18 03:00:06 2026 GMT
  host: www.starwoodhotels.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Starwood Hotels And Resorts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Starwood Hotels and Resorts, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Starwood Hotels and Resorts
provider_slug: starwood-hotels-and-resorts
slug: starwood-hotels-and-resorts-domain-security
source_filename: starwood-hotels-and-resorts-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.starwoodhotels.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 03:00:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: starwoodhotels.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/starwood-hotels-and-resorts/refs/heads/main/security/starwood-hotels-and-resorts-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
