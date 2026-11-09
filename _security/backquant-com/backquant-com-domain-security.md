---
api_specs:
- filename: backquant-com-api-openapi.json
  format: json
  label: BackQuant API v2 API
  slug: backquant-api-v2-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backquant-com/openapi/_original/backquant-com-api-openapi.json
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: backquant.com
  spf: true
hosts:
- cert_expires: Dec 30 06:19:04 2026 GMT
  host: backquant.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Backquant Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BackQuant, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BackQuant
provider_slug: backquant-com
slug: backquant-com-domain-security
source_filename: backquant-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: backquant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 06:19:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: backquant.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/backquant-com/security/backquant-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Trading
- Options
- Cryptocurrency
- Analytics
---
