---
api_specs:
- filename: justifi-openapi-original.yml
  format: yaml
  label: JustiFi API
  slug: justifi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justifi/refs/heads/main/openapi/justifi-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: justifi.ai
  spf: true
hosts:
- cert_expires: Sep 24 03:06:39 2026 GMT
  host: www.justifi.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 11 23:59:59 2027 GMT
  host: api.justifi.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Justifi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JustiFi, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: JustiFi
provider_slug: justifi
slug: justifi-domain-security
source_filename: justifi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.justifi.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 03:06:39 2026 GMT\n  hsts: null\n- host: api.justifi.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 11 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: justifi.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/justifi/refs/heads/main/security/justifi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Payments
- Embedded Payments
- Payment Facilitation
- Payouts
- Developers
- API
---
