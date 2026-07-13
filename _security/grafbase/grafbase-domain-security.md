---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: grafbase.com
  spf: false
hosts:
- cert_expires: Sep 24 20:50:45 2026 GMT
  host: grafbase.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 18:38:29 2026 GMT
  host: api.grafbase.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Grafbase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Grafbase, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Grafbase
provider_slug: grafbase
slug: grafbase-domain-security
source_filename: grafbase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: grafbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 20:50:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.grafbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 18:38:29 2026 GMT\n  hsts: null\ndomains:\n- domain: grafbase.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grafbase/refs/heads/main/security/grafbase-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- GraphQL
- Federation
- API Gateway
- Schema Registry
- GraphQL Federation
- API Management
- Observability
- Enterprise API
---
