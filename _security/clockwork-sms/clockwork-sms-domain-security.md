---
api_specs:
- filename: clockwork-sms-openapi-generated.yml
  format: yaml
  label: Clockwork SMS API
  slug: clockwork-sms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clockwork-sms/openapi/_ae-authored/clockwork-sms-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: textanywhere.com
  spf: true
hosts:
- cert_expires: Feb 12 05:33:00 2027 GMT
  host: textanywhere.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Clockwork SMS Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clockwork SMS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Clockwork SMS
provider_slug: clockwork-sms
slug: clockwork-sms-domain-security
source_filename: clockwork-sms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: textanywhere.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 05:33:00 2027 GMT\n  hsts: false\ndomains:\n- domain: textanywhere.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/clockwork-sms/security/clockwork-sms-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- SMS
- Marketing
- United Kingdom
- Communications
---
