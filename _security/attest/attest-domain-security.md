---
api_specs:
- filename: attest-studies-api-openapi.yml
  format: yaml
  label: Attest Studies API
  slug: attest-studies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attest/refs/heads/main/openapi/attest-studies-api-openapi.yml
- filename: attest-study-api-openapi.yml
  format: yaml
  label: Attest Study API
  slug: attest-study-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attest/refs/heads/main/openapi/attest-study-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: askattest.com
  spf: true
hosts:
- cert_expires: Nov 13 18:57:19 2026 GMT
  host: www.askattest.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Attest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Attest, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Attest
provider_slug: attest
slug: attest-domain-security
source_filename: attest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.askattest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 18:57:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: askattest.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/attest/refs/heads/main/security/attest-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Consumer Insights
- Market Research
- Consumer
- Analytics
---
