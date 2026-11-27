---
api_specs:
- filename: getinfrly-com-openapi-generated.yml
  format: yaml
  label: Infrly API
  slug: getinfrly-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getinfrly-com/openapi/_ae-authored/getinfrly-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getinfrly.com
  spf: true
hosts:
- cert_expires: Dec 29 08:12:08 2026 GMT
  host: getinfrly.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Infrly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Infrly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Infrly
provider_slug: getinfrly-com
slug: getinfrly-com-domain-security
source_filename: getinfrly-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getinfrly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 08:12:08 2026 GMT\n  hsts: false\ndomains:\n- domain: getinfrly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/getinfrly-com/security/getinfrly-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Platform-as-a-Service
- Deployment
- Web App
- Static Sites
- PostgreSQL
- Open Source
---
