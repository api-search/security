---
api_specs:
- filename: interpol-notices-api-openapi.yml
  format: yaml
  label: Interpol Notices API
  slug: interpol-notices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interpol/refs/heads/main/openapi/interpol-notices-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: interpol.int
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: bund.dev
  spf: false
hosts:
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: www.interpol.int
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 05:48:20 2026 GMT
  host: interpol.api.bund.dev
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: ws-public.interpol.int
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Interpol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Interpol, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Interpol
provider_slug: interpol
slug: interpol-domain-security
source_filename: interpol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.interpol.int\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: interpol.api.bund.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 05:48:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: ws-public.interpol.int\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: interpol.int\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: bund.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/interpol/refs/heads/main/security/interpol-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Federal-Government
- International
- Law Enforcement
- Notices
- Police
---
