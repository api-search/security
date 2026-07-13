---
api_specs:
- filename: sex-offenders-api-openapi.yml
  format: yaml
  label: Sex Offenders API
  slug: sex-offenders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sex-offenders-api/refs/heads/main/openapi/sex-offenders-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: crimeometer.com
  spf: true
hosts:
- cert_expires: Sep 17 18:28:48 2026 GMT
  host: www.crimeometer.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: api.crimeometer.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sex Offenders Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sex Offenders API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sex Offenders API
provider_slug: sex-offenders-api
slug: sex-offenders-api-domain-security
source_filename: sex-offenders-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.crimeometer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 18:28:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: api.crimeometer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: crimeometer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sex-offenders-api/refs/heads/main/security/sex-offenders-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sex Offenders
---
