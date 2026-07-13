---
api_specs:
- filename: farm-machinery-and-equipment-api-openapi.yml
  format: yaml
  label: Farm Machinery and Equipment API
  slug: farm-machinery-and-equipment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farm-machinery-and-equipment-api/refs/heads/main/openapi/farm-machinery-and-equipment-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apifarmer.com
  spf: true
hosts:
- cert_expires: Aug 31 02:24:01 2026 GMT
  host: apifarmer.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.apifarmer.com
  https: false
kind: domain-security
layout: security
method: probed
name: Farm Machinery And Equipment Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Farm Machinery and Equipment API, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Farm Machinery and Equipment API
provider_slug: farm-machinery-and-equipment-api
slug: farm-machinery-and-equipment-api-domain-security
source_filename: farm-machinery-and-equipment-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apifarmer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 02:24:01 2026 GMT\n  hsts: false\n- host: api.apifarmer.com\n  https: false\ndomains:\n- domain: apifarmer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/farm-machinery-and-equipment-api/refs/heads/main/security/farm-machinery-and-equipment-api-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Equipment
- Farms
- Machinery
---
