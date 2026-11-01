---
api_specs:
- filename: appsignal-openapi-generated.yml
  format: yaml
  label: AppSignal API
  slug: appsignal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appsignal/openapi/_ae-authored/appsignal-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: appsignal.com
  spf: true
hosts:
- cert_expires: Jan 16 02:18:36 2027 GMT
  host: www.appsignal.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Appsignal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AppSignal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AppSignal
provider_slug: appsignal
slug: appsignal-domain-security
source_filename: appsignal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.appsignal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 02:18:36 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: appsignal.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/appsignal/security/appsignal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Monitoring
- ErrorTracking
- Performance
- Observability
- SaaS
---
