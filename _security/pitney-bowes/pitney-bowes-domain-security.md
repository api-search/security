---
api_specs:
- filename: pitney-bowes-openapi.yml
  format: yaml
  label: Pitney Bowes APIs
  slug: pitney-bowes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pitney-bowes/refs/heads/main/openapi/pitney-bowes-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: pitneybowes.com
  spf: false
hosts:
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: docs.shippingapi.pitneybowes.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Mar  9 23:59:59 2027 GMT
  host: shipping-api.pitneybowes.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  9 23:59:59 2027 GMT
  host: shipping-api-sandbox.pitneybowes.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pitney Bowes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pitney Bowes, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=reject).'
provider_name: Pitney Bowes
provider_slug: pitney-bowes
slug: pitney-bowes-domain-security
source_filename: pitney-bowes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.shippingapi.pitneybowes.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: false\n- host: shipping-api.pitneybowes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  9 23:59:59 2027 GMT\n  hsts: null\n- host: shipping-api-sandbox.pitneybowes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  9 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: pitneybowes.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pitney-bowes/refs/heads/main/security/pitney-bowes-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Mailing
- Shipping
- Fortune 1000
---
