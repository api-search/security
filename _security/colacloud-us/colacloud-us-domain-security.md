---
api_specs:
- filename: colacloud-us-colas-api-openapi.yml
  format: yaml
  label: COLA Cloud COLAs API
  slug: colacloud-us-colas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/colacloud-us/openapi/colacloud-us-colas-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: colacloud.us
  spf: true
hosts:
- cert_expires: Dec 29 04:00:18 2026 GMT
  host: colacloud.us
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: COLA Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for COLA Cloud, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: COLA Cloud
provider_slug: colacloud-us
slug: colacloud-us-domain-security
source_filename: colacloud-us-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: colacloud.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 04:00:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: colacloud.us\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/colacloud-us/security/colacloud-us-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data
- Alcohol
- Compliance
- Open Data
---
