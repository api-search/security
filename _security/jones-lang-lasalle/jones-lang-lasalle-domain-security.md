---
api_specs:
- filename: jones-lang-lasalle-corrigo-rest-api-openapi.yml
  format: yaml
  label: JLL Corrigo Enterprise REST API
  slug: corrigo-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jones-lang-lasalle/refs/heads/main/openapi/jones-lang-lasalle-corrigo-rest-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jll.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: corrigo.com
  spf: true
hosts:
- cert_expires: Feb 17 23:59:59 2027 GMT
  host: www.jll.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 16:39:08 2026 GMT
  host: developer.corrigo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: am-ce98c.corrigo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jones Lang Lasalle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jones Lang LaSalle, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Jones Lang LaSalle
provider_slug: jones-lang-lasalle
slug: jones-lang-lasalle-domain-security
source_filename: jones-lang-lasalle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jll.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: developer.corrigo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 16:39:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: am-ce98c.corrigo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: jll.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: corrigo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jones-lang-lasalle/refs/heads/main/security/jones-lang-lasalle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Commercial Real Estate
- Facility Management
- Asset Management
- Work Orders
- Fortune 500
---
