---
api_specs:
- filename: jojapi-openapi-generated.yml
  format: yaml
  label: APRYCO API
  slug: jojapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jojapi/refs/heads/main/openapi/_ae-authored/jojapi-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jojapi.com
  spf: true
hosts:
- cert_expires: Dec 28 05:07:03 2026 GMT
  host: jojapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jojapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for APRYCO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: APRYCO
provider_slug: jojapi
slug: jojapi-domain-security
source_filename: jojapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jojapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 05:07:03 2026 GMT\n  hsts: false\ndomains:\n- domain: jojapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jojapi/refs/heads/main/security/jojapi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Marketplace
- Data
- Scraping
- APIs
---
