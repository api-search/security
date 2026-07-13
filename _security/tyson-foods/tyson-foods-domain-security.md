---
api_specs:
- filename: tyson-foods-edi-integration-api-openapi.yml
  format: yaml
  label: Tyson Foods EDI Integration API
  slug: tyson-foods-edi-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyson-foods/refs/heads/main/openapi/tyson-foods-edi-integration-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tysonfoods.com
  spf: false
hosts:
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: www.tysonfoods.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.tysonfoods.com
  https: false
kind: domain-security
layout: security
method: probed
name: Tyson Foods Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tyson Foods, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Tyson Foods
provider_slug: tyson-foods
slug: tyson-foods-domain-security
source_filename: tyson-foods-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tysonfoods.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: false\n- host: api.tysonfoods.com\n  https: false\ndomains:\n- domain: tysonfoods.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tyson-foods/refs/heads/main/security/tyson-foods-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- B2B Integration
- EDI
- Food
- Fortune 100
- Supply Chain
---
