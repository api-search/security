---
api_specs:
- filename: kth-swagger-openapi.json
  format: json
  label: KTH Royal Institute of Technology Swagger API
  slug: kth-royal-institute-of-technology-swagger-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kth/refs/heads/main/openapi/_original/kth-swagger-openapi.json
- filename: kth-swagger-openapi.json
  format: json
  label: KTH Royal Institute of Technology Swagger API
  slug: kth-royal-institute-of-technology-swagger-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kth/refs/heads/main/openapi/_original/kth-swagger-openapi.json
description: ''
domains:
- caa:
  - 0 issue "harica.gr"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: kth.se
  spf: true
hosts:
- cert_expires: Feb 27 07:45:29 2027 GMT
  host: kth.se
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KTH Royal Institute of Technology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: KTH Royal Institute of Technology
provider_slug: kth
slug: kth-domain-security
source_filename: kth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kth.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 07:45:29 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: kth.se\n  dnssec: true\n  caa:\n  - 0 issue \"harica.gr\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kth/refs/heads/main/security/kth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Education
- Research
- Sweden
- Technology
---
