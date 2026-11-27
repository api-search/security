---
api_specs:
- filename: tallinn-ee-data-api-openapi.yml
  format: yaml
  label: Tallinn Data API
  slug: tallinn-ee-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tallinn-ee/openapi/tallinn-ee-data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tallinn.ee
  spf: true
hosts:
- cert_expires: Jan 17 17:25:36 2027 GMT
  host: www.tallinn.ee
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tallinn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tallinn, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tallinn
provider_slug: tallinn-ee
slug: tallinn-ee-domain-security
source_filename: tallinn-ee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tallinn.ee\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 17:25:36 2027 GMT\n  hsts: null\ndomains:\n- domain: tallinn.ee\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/tallinn-ee/security/tallinn-ee-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Government
- Municipal
- Open Data
- Estonia
- Smart City
- Public Sector
---
