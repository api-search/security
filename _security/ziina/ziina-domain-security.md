---
api_specs:
- filename: ziina-openapi.yml
  format: yaml
  label: Ziina Payment Intent API
  slug: ziina-payment-intent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ziina/refs/heads/main/openapi/ziina-openapi.yml
- filename: ziina-openapi.yml
  format: yaml
  label: Ziina Refund API
  slug: ziina-refund-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ziina/refs/heads/main/openapi/ziina-openapi.yml
- filename: ziina-openapi.yml
  format: yaml
  label: Ziina Transfer API
  slug: ziina-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ziina/refs/heads/main/openapi/ziina-openapi.yml
- filename: ziina-openapi.yml
  format: yaml
  label: Ziina Webhooks API
  slug: ziina-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ziina/refs/heads/main/openapi/ziina-openapi.yml
- filename: ziina-openapi.yml
  format: yaml
  label: Ziina Account API
  slug: ziina-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ziina/refs/heads/main/openapi/ziina-openapi.yml
description: ''
domains:
- caa: []
  caa_note: No CAA records published for ziina.com (DNS fronted by Cloudflare).
  dmarc: true
  dmarc_note: p=none with strict alignment (adkim=s; aspf=s) and rua reporting to dmarc-reports.cloudflare.net and dev@ziina.com.
  dmarc_policy: none
  dnssec: false
  domain: ziina.com
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:spf.mailjet.com include:amazonses.com -all
hosts:
- cert_expires: Sep 18 08:18:35 2026 GMT
  host: ziina.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 09:53:32 2026 GMT
  host: api-v2.ziina.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15552000
  https: true
  note: Bare GET / returns HTTP 400 (API host, expects authenticated API calls).
  tls_version: TLSv1.3
- cert_expires: Oct 10 09:53:32 2026 GMT
  host: auth.ziina.com
  hsts: false
  https: true
  note: OAuth 2.0 / OIDC authorization server (auth.ziina.com/oidc).
  tls_version: TLSv1.3
- cert_expires: Aug 28 00:15:06 2026 GMT
  host: docs.ziina.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ziina Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ziina, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ziina
provider_slug: ziina
slug: ziina-domain-security
source_filename: ziina-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ziina.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 08:18:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api-v2.ziina.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 09:53:32 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n  hsts_include_subdomains: true\n  note: Bare GET / returns HTTP 400 (API host, expects authenticated API calls).\n- host: auth.ziina.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 09:53:32 2026 GMT\n  hsts: false\n  note: OAuth 2.0 / OIDC authorization server (auth.ziina.com/oidc).\n- host: docs.ziina.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 00:15:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ziina.com\n  dnssec: false\n  caa: []\n  caa_note: No CAA records published for ziina.com (DNS fronted by Cloudflare).\n\
  \  spf: true\n  spf_record: v=spf1 include:_spf.google.com include:spf.mailjet.com include:amazonses.com -all\n  dmarc: true\n  dmarc_policy: none\n  dmarc_note: >-\n    p=none with strict alignment (adkim=s; aspf=s) and rua reporting to\n    dmarc-reports.cloudflare.net and dev@ziina.com.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ziina/refs/heads/main/security/ziina-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Fintech
- UAE
- MENA
- Money Transfer
- Wallet
---
