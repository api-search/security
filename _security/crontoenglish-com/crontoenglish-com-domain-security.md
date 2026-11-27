---
api_specs:
- filename: crontoenglish-com-build-api-openapi.yml
  format: yaml
  label: Cron Translator Build API
  slug: crontoenglish-com-build-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crontoenglish-com/openapi/crontoenglish-com-build-api-openapi.yml
- filename: crontoenglish-com-explain-api-openapi.yml
  format: yaml
  label: Cron Translator Explain API
  slug: crontoenglish-com-explain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crontoenglish-com/openapi/crontoenglish-com-explain-api-openapi.yml
- filename: crontoenglish-com-next-runs-api-openapi.yml
  format: yaml
  label: Cron Translator Next Runs API
  slug: crontoenglish-com-next-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crontoenglish-com/openapi/crontoenglish-com-next-runs-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: crontoenglish.com
  spf: false
hosts:
- cert_expires: Feb  1 08:34:34 2027 GMT
  host: crontoenglish.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cron Translator Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cron Translator, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Cron Translator
provider_slug: crontoenglish-com
slug: crontoenglish-com-domain-security
source_filename: crontoenglish-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crontoenglish.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 08:34:34 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: crontoenglish.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/crontoenglish-com/security/crontoenglish-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Cron
- Translator
- CronExpressions
- Scheduler
---
