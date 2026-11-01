---
api_specs:
- filename: inboxpolicy-com-verification-api-openapi.yml
  format: yaml
  label: inboxpolicy-com Verification API
  slug: inboxpolicy-com-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxpolicy-com/openapi/inboxpolicy-com-verification-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: inboxpolicy.com
  spf: true
hosts:
- cert_expires: Jan 27 13:28:54 2027 GMT
  host: inboxpolicy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Inboxpolicy Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for inboxpolicy-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: inboxpolicy-com
provider_slug: inboxpolicy-com
slug: inboxpolicy-com-domain-security
source_filename: inboxpolicy-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inboxpolicy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 13:28:54 2027 GMT\n  hsts: false\ndomains:\n- domain: inboxpolicy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/inboxpolicy-com/security/inboxpolicy-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- EmailVerification
- API
- AI
- Payments
- Pricing
---
