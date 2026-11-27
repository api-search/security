---
api_specs:
- filename: mobiscroll-com-openapi-generated.yml
  format: yaml
  label: Mobiscroll API
  slug: mobiscroll-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mobiscroll-com/openapi/_ae-authored/mobiscroll-com-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com"
  - 0 iodef "mailto:support@mobiscroll.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mobiscroll.com
  spf: true
hosts:
- cert_expires: Apr 25 23:59:59 2027 GMT
  host: mobiscroll.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mobiscroll Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mobiscroll, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mobiscroll
provider_slug: mobiscroll-com
slug: mobiscroll-com-domain-security
source_filename: mobiscroll-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mobiscroll.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 25 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mobiscroll.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 iodef \"mailto:support@mobiscroll.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/mobiscroll-com/security/mobiscroll-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- UI
- Scheduling
- Calendar
- JavaScript
- OpenAPI
---
