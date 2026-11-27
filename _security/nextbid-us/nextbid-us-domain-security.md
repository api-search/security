---
api_specs:
- filename: nextbid-us-account-api-openapi.yml
  format: yaml
  label: NextBid Account API
  slug: nextbid-us-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nextbid-us/openapi/nextbid-us-account-api-openapi.yml
- filename: nextbid-us-health-api-openapi.yml
  format: yaml
  label: NextBid Health API
  slug: nextbid-us-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nextbid-us/openapi/nextbid-us-health-api-openapi.yml
- filename: nextbid-us-opportunities-api-openapi.yml
  format: yaml
  label: NextBid Opportunities API
  slug: nextbid-us-opportunities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nextbid-us/openapi/nextbid-us-opportunities-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nextbid.us
  spf: true
hosts:
- cert_expires: Jan 12 12:26:27 2027 GMT
  host: nextbid.us
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: NextBid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NextBid, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: NextBid
provider_slug: nextbid-us
slug: nextbid-us-domain-security
source_filename: nextbid-us-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nextbid.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 12:26:27 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nextbid.us\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/nextbid-us/security/nextbid-us-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Government Bids
- Small Business
- Procurement
- Artificial Intelligence
- Set‑asides
---
