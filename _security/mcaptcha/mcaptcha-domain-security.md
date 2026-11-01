---
api_specs:
- filename: mcaptcha-openapi.yml
  format: yaml
  label: mCaptcha Guard API
  slug: mcaptcha-guard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcaptcha/openapi/mcaptcha-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: mcaptcha.org
  spf: true
hosts:
- cert_expires: Jan 14 12:08:24 2027 GMT
  host: mcaptcha.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mcaptcha Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mCaptcha, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: mCaptcha
provider_slug: mcaptcha
slug: mcaptcha-domain-security
source_filename: mcaptcha-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mcaptcha.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 12:08:24 2027 GMT\n  hsts: false\ndomains:\n- domain: mcaptcha.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/mcaptcha/security/mcaptcha-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Captcha
- Privacy
- OpenSource
- PoW
- Security
---
