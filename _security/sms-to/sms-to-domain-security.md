---
api_specs:
- filename: sms-to-openapi-generated.yml
  format: yaml
  label: SMS.to API
  slug: sms-to-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sms-to/openapi/_ae-authored/sms-to-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sms.to
  spf: true
hosts:
- cert_expires: Jan 14 09:14:58 2027 GMT
  host: sms.to
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: SMS.to Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SMS.to, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SMS.to
provider_slug: sms-to
slug: sms-to-domain-security
source_filename: sms-to-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sms.to\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 09:14:58 2027 GMT\n  hsts: false\ndomains:\n- domain: sms.to\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/sms-to/security/sms-to-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- SMS
- Messaging API
- Omnichannel Messaging
- Bulk SMS
- Verification
- HLR
- Viber Messaging
---
