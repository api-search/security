---
api_specs:
- filename: 2captcha-2captcha-api-api-openapi.yml
  format: yaml
  label: 2Captcha API
  slug: 2captcha-api-2
  spec_type: OpenAPI
  url: https://artifacts.apis.io/2captcha/openapi/2captcha-2captcha-api-api-openapi.yml
- filename: 2captcha-openapi-generated.yml
  format: yaml
  label: 2captcha API
  slug: 2captcha-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/2captcha/openapi/_ae-authored/2captcha-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 2captcha.com
  spf: true
hosts:
- cert_expires: Dec  9 05:24:36 2026 GMT
  host: 2captcha.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 2Captcha Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 2captcha, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 2captcha
provider_slug: 2captcha
slug: 2captcha-domain-security
source_filename: 2captcha-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 2captcha.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 05:24:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 2captcha.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/2captcha/security/2captcha-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Captcha Solving
- API
- Automation
- Web Scraping
- Data Extraction
---
