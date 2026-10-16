---
api_specs:
- filename: ex-libris-openapi-generated.yml
  format: yaml
  label: Ex Libris API
  slug: ex-libris-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ex-libris/refs/heads/main/openapi/_ae-authored/ex-libris-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: exlibrisgroup.com
  spf: true
hosts:
- cert_expires: Dec  6 20:28:18 2026 GMT
  host: www.exlibrisgroup.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ex Libris Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ex Libris, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ex Libris
provider_slug: ex-libris
slug: ex-libris-domain-security
source_filename: ex-libris-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.exlibrisgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 20:28:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: exlibrisgroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ex-libris/refs/heads/main/security/ex-libris-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Library
- Software
- Academic
- Cloud
- Solutions
---
