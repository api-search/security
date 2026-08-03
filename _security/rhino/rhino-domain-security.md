---
api_specs:
- filename: rhino-partner-api-openapi.json
  format: json
  label: SayRhino Partner API
  slug: sayrhino-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhino/refs/heads/main/openapi/rhino-partner-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sayrhino.com
  spf: true
hosts:
- cert_expires: Sep 30 01:43:29 2026 GMT
  host: www.sayrhino.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: api.prod.sayrhino.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rhino Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rhino, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rhino
provider_slug: rhino
slug: rhino-domain-security
source_filename: rhino-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sayrhino.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 01:43:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.prod.sayrhino.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sayrhino.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rhino/refs/heads/main/security/rhino-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Insurtech
- Real Estate
- Property Management
- Rentals
- Security Deposits
- Renters Insurance
- Webhooks
- Partner API
---
