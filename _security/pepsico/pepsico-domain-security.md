---
api_specs:
- filename: pepsico-pepsico-api-openapi.yml
  format: yaml
  label: PepsiCo API
  slug: pepsico-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pepsico/refs/heads/main/openapi/pepsico-pepsico-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pepsico.com
  spf: true
hosts:
- cert_expires: Sep 21 23:59:59 2026 GMT
  host: www.pepsico.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.pepsico.com
  https: false
kind: domain-security
layout: security
method: probed
name: Pepsico Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PepsiCo, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PepsiCo
provider_slug: pepsico
slug: pepsico-domain-security
source_filename: pepsico-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pepsico.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 23:59:59 2026 GMT\n  hsts: null\n- host: api.pepsico.com\n  https: false\ndomains:\n- domain: pepsico.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pepsico/refs/heads/main/security/pepsico-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Beverages
- Food
- Retail
- Supply Chain
- Fortune 100
---
