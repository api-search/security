---
api_specs:
- filename: asapio-openapi-generated.yml
  format: yaml
  label: ASAPIO API
  slug: asapio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapio/refs/heads/main/openapi/_ae-authored/asapio-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: asapio.com
  spf: true
hosts:
- cert_expires: Apr  3 23:59:59 2027 GMT
  host: asapio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Asapio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ASAPIO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ASAPIO
provider_slug: asapio
slug: asapio-domain-security
source_filename: asapio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: asapio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  3 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: asapio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asapio/refs/heads/main/security/asapio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- SAP
- Integration
- Cloud
- API
- Enterprise
---
