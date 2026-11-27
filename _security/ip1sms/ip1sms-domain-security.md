---
api_specs:
- filename: ip1sms-openapi-generated.yml
  format: yaml
  label: iP1 SMS API
  slug: ip1sms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ip1sms/openapi/_ae-authored/ip1sms-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ip1sms.com
  spf: true
hosts:
- cert_expires: Jan 28 02:03:59 2027 GMT
  host: ip1sms.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: iP1 SMS Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iP1 SMS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: iP1 SMS
provider_slug: ip1sms
slug: ip1sms-domain-security
source_filename: ip1sms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ip1sms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 02:03:59 2027 GMT\n  hsts: false\ndomains:\n- domain: ip1sms.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/ip1sms/security/ip1sms-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- SMS
- Communications
- Enterprise
- Integration
---
