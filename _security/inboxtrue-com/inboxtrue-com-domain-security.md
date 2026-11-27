---
api_specs:
- filename: inboxtrue-com-email-api-openapi.yml
  format: yaml
  label: InboxTrue Email API
  slug: inboxtrue-com-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxtrue-com/openapi/inboxtrue-com-email-api-openapi.yml
- filename: inboxtrue-com-zeroclick-api-openapi.yml
  format: yaml
  label: InboxTrue Zeroclick API
  slug: inboxtrue-com-zeroclick-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxtrue-com/openapi/inboxtrue-com-zeroclick-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: inboxtrue.com
  spf: true
hosts:
- cert_expires: Jan 21 12:07:28 2027 GMT
  host: inboxtrue.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: InboxTrue Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for InboxTrue, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: InboxTrue
provider_slug: inboxtrue-com
slug: inboxtrue-com-domain-security
source_filename: inboxtrue-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inboxtrue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 12:07:28 2027 GMT\n  hsts: false\ndomains:\n- domain: inboxtrue.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/inboxtrue-com/security/inboxtrue-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Email Verification
- Software-as-a-Service
- Developer Tools
---
