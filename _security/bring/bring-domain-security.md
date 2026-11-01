---
api_specs:
- filename: bring-openapi-generated.yml
  format: yaml
  label: Bring API
  slug: bring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bring/openapi/_ae-authored/bring-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bring.com
  spf: true
hosts:
- cert_expires: Dec 22 19:52:48 2026 GMT
  host: bring.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bring Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bring, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Bring
provider_slug: bring
slug: bring-domain-security
source_filename: bring-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bring.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 19:52:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: bring.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/bring/security/bring-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Logistics
- Shipping
- E‑commerce
- API
- Norway
---
