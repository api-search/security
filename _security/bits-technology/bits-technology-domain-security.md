---
api_specs:
- filename: bits-technology-openapi-generated.yml
  format: yaml
  label: Bits Technology API
  slug: bits-technology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bits-technology/refs/heads/main/openapi/_ae-authored/bits-technology-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "certainly.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bits.bi
  spf: true
hosts:
- cert_expires: Nov 23 23:06:39 2026 GMT
  host: bits.bi
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bits Technology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bits Technology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bits Technology
provider_slug: bits-technology
slug: bits-technology-domain-security
source_filename: bits-technology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bits.bi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 23:06:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bits.bi\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bits-technology/refs/heads/main/security/bits-technology-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AML
- Compliance
- Fintech
- Europe
---
