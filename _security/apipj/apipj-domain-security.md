---
api_specs:
- filename: apipj-api-openapi.json
  format: json
  label: apipj API
  slug: apipj-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apipj/refs/heads/main/openapi/_original/apipj-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: apipj.com.br
  spf: false
hosts:
- cert_expires: Jan  7 20:08:31 2027 GMT
  host: apipj.com.br
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Apipj Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for apipj (MASTER BI TECNOLOGIA LTDA), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: apipj (MASTER BI TECNOLOGIA LTDA)
provider_slug: apipj
slug: apipj-domain-security
source_filename: apipj-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apipj.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 20:08:31 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apipj.com.br\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apipj/refs/heads/main/security/apipj-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Brazil
- CNPJ
- Registry
- Public API
---
