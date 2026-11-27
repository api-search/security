---
api_specs:
- filename: sms-hosting-openapi-generated.yml
  format: yaml
  label: SMS Hosting API
  slug: sms-hosting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sms-hosting/openapi/_ae-authored/sms-hosting-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: smshosting.it
  spf: true
hosts:
- cert_expires: Feb  1 06:39:45 2027 GMT
  host: smshosting.it
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: SMS Hosting Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SMS Hosting, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SMS Hosting
provider_slug: sms-hosting
slug: sms-hosting-domain-security
source_filename: sms-hosting-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: smshosting.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 06:39:45 2027 GMT\n  hsts: false\ndomains:\n- domain: smshosting.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/sms-hosting/security/sms-hosting-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Communications
- Messaging
- Marketing
- SMS
- Multi-Channel
---
