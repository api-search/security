---
api_specs:
- filename: adios-hr-radar-api-api-openapi.yml
  format: yaml
  label: adios-hr Radar API
  slug: adios-hr-radar-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adios-hr/openapi/adios-hr-radar-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: adios.hr
  spf: true
hosts:
- cert_expires: Dec  5 04:39:01 2026 GMT
  host: adios.hr
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: adios-hr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for adios-hr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: adios-hr
provider_slug: adios-hr
slug: adios-hr-domain-security
source_filename: adios-hr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adios.hr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 04:39:01 2026 GMT\n  hsts: null\ndomains:\n- domain: adios.hr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/adios-hr/security/adios-hr-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
