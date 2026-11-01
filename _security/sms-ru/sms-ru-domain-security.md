---
api_specs:
- filename: sms-ru-openapi-generated.yml
  format: yaml
  label: SMS.ru API
  slug: sms-ru-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sms-ru/openapi/_ae-authored/sms-ru-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sms.ru
  spf: true
hosts:
- cert_expires: Jan 23 03:00:57 2027 GMT
  host: sms.ru
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sms Ru Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SMS.ru, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SMS.ru
provider_slug: sms-ru
slug: sms-ru-domain-security
source_filename: sms-ru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sms.ru\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 03:00:57 2027 GMT\n  hsts: false\ndomains:\n- domain: sms.ru\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/sms-ru/security/sms-ru-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- SMS
- Messaging
- API
- Russia
---
