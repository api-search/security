---
api_specs:
- filename: appsumo-licensing-openapi.yaml
  format: yaml
  label: AppSumo Licensing API
  slug: appsumo-licensing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsumo/refs/heads/main/openapi/appsumo-licensing-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: appsumo.com
  spf: true
hosts:
- cert_expires: Aug 11 22:59:53 2026 GMT
  host: appsumo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: docs.licensing.appsumo.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Appsumo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AppSumo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AppSumo
provider_slug: appsumo
slug: appsumo-domain-security
source_filename: appsumo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: appsumo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 22:59:53 2026 GMT\n  hsts: false\n- host: docs.licensing.appsumo.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: appsumo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appsumo/refs/heads/main/security/appsumo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Marketplace
- SaaS
- Software Deals
---
