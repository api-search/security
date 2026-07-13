---
api_specs:
- filename: openapi
  format: yaml
  label: Chargebee API v2
  slug: chargebee-api
  spec_type: OpenAPI
  url: https://github.com/chargebee/openapi
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: chargebee.com
  spf: true
hosts:
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: www.chargebee.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 14 23:59:59 2026 GMT
  host: apidocs.chargebee.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chargebee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chargebee, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Chargebee
provider_slug: chargebee
slug: chargebee-domain-security
source_filename: chargebee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chargebee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: apidocs.chargebee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: chargebee.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chargebee/refs/heads/main/security/chargebee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Billing
- Subscriptions
- Recurring Billing
- Revenue
- Payments
- SaaS
---
