---
api_specs:
- filename: bluestacks-payments-asyncapi.yml
  format: yaml
  label: now.gg Payments Server API
  slug: nowgg-payments-server-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluestacks/refs/heads/main/asyncapi/bluestacks-payments-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bluestacks.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: now.gg
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bluestacks.ai
  spf: false
hosts:
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: www.bluestacks.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: docs.now.gg
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: now.gg
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: payments-api.now.gg
  hsts: true
  hsts_max_age: 2592000
  https: true
  note: HSTS max-age is 30 days, below the 1-year threshold browsers require for preload.
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: studio.now.gg
  hsts: false
  https: true
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: bluestacks.ai
  hsts: false
  https: true
kind: domain-security
layout: security
method: probed
name: Bluestacks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bluestacks, probed live across 6 host(s) and 3 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bluestacks
provider_slug: bluestacks
slug: bluestacks-domain-security
source_filename: bluestacks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bluestacks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.now.gg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: now.gg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: false\n- host: payments-api.now.gg\n  https: true\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\n  note: HSTS max-age is 30 days, below the 1-year threshold browsers require for preload.\n- host: studio.now.gg\n  https: true\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: false\n- host: bluestacks.ai\n  https: true\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: bluestacks.com\n  dnssec: false\n  caa: []\n  spf:\
  \ true\n  dmarc: true\n  dmarc_policy: reject\n- domain: now.gg\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: bluestacks.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\nx-evidence:\n  probed: '2026-08-08'\n  method: openssl s_client + curl HEAD + dig\n  hosts_probed: 6\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluestacks/refs/heads/main/security/bluestacks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Gaming
- Cloud Gaming
- Android
- Mobile
- Payments
- In-App Purchases
- Subscriptions
- Developer Platform
- App Distribution
- Advertising
- OAuth
---
