---
api_specs:
- filename: htmlweb-ru-json-api-openapi.yml
  format: yaml
  label: htmlweb-ru JSON API
  slug: htmlweb-ru-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/htmlweb-ru/openapi/htmlweb-ru-json-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: htmlweb.ru
  spf: true
hosts:
- cert_expires: Jan 16 23:19:40 2027 GMT
  host: htmlweb.ru
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Htmlweb Ru Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for htmlweb-ru, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: htmlweb-ru
provider_slug: htmlweb-ru
slug: htmlweb-ru-domain-security
source_filename: htmlweb-ru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: htmlweb.ru\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 16 23:19:40 2027 GMT\n  hsts: false\ndomains:\n- domain: htmlweb.ru\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/htmlweb-ru/security/htmlweb-ru-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Web
- API
- Russia
- Data
- Utilities
---
