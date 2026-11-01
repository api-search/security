---
api_specs:
- filename: dataddo-openapi-generated.yml
  format: yaml
  label: Dataddo API
  slug: dataddo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataddo/openapi/_ae-authored/dataddo-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: dataddo.com
  spf: true
hosts:
- cert_expires: Dec  8 17:20:45 2026 GMT
  host: dataddo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dataddo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dataddo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Dataddo
provider_slug: dataddo
slug: dataddo-domain-security
source_filename: dataddo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dataddo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 17:20:45 2026 GMT\n  hsts: false\ndomains:\n- domain: dataddo.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dataddo/security/dataddo-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Data Integration
- API Platform
- Artificial Intelligence
- Real-Time
- ETL
---
