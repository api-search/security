---
api_specs:
- filename: outsend-xyz-openapi-generated.yml
  format: yaml
  label: Outsend API
  slug: outsend-xyz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outsend-xyz/openapi/_ae-authored/outsend-xyz-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: outsend.xyz
  spf: true
hosts:
- cert_expires: Jan 29 21:51:42 2027 GMT
  host: outsend.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Outsend Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Outsend, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Outsend
provider_slug: outsend-xyz
slug: outsend-xyz-domain-security
source_filename: outsend-xyz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: outsend.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 21:51:42 2027 GMT\n  hsts: null\ndomains:\n- domain: outsend.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/outsend-xyz/security/outsend-xyz-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- B2B
- Prospecting
- Data Enrichment
- Web Scraping
---
