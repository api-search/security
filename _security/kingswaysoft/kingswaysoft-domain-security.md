---
api_specs:
- filename: kingswaysoft-openapi-generated.yml
  format: yaml
  label: KingswaySoft API
  slug: kingswaysoft-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kingswaysoft/openapi/_ae-authored/kingswaysoft-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: kingswaysoft.com
  spf: true
hosts:
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: kingswaysoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kingswaysoft Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KingswaySoft, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: KingswaySoft
provider_slug: kingswaysoft
slug: kingswaysoft-domain-security
source_filename: kingswaysoft-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kingswaysoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kingswaysoft.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/kingswaysoft/security/kingswaysoft-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Data Integration
- ETL
- Microsoft SSIS
- Connectors
- Enterprise
---
