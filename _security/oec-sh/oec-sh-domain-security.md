---
api_specs:
- filename: oec-sh-api-openapi.json
  format: json
  label: OEC.sh Api API
  slug: oec-sh-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oec-sh/openapi/_original/oec-sh-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: oec.sh
  spf: true
hosts:
- cert_expires: Dec 27 15:42:17 2026 GMT
  host: oec.sh
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OpenEduCat Inc. Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenEduCat Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OpenEduCat Inc.
provider_slug: oec-sh
slug: oec-sh-domain-security
source_filename: oec-sh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oec.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 15:42:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: oec.sh\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/oec-sh/security/oec-sh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Odoo
- Hosting
- Software-as-a-Service
- Cloud
- Open Source
---
