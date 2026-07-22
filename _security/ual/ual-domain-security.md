---
api_specs:
- filename: ual-bis-cobros-online-v2-openapi.yml
  format: yaml
  label: Ualá Bis API Cobros Online v2
  slug: ualá-bis-api-cobros-online-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ual/refs/heads/main/openapi/ual-bis-cobros-online-v2-openapi.yml
- filename: ual-bis-auth-v2-openapi.yml
  format: yaml
  label: Ualá Bis Authentication API v2
  slug: ualá-bis-authentication-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ual/refs/heads/main/openapi/ual-bis-auth-v2-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: uala.com.ar
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ualabis.com.ar
  spf: true
hosts:
- cert_expires: Oct  1 20:17:19 2026 GMT
  host: www.uala.com.ar
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 02:29:12 2026 GMT
  host: developers.ualabis.com.ar
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 20:17:19 2026 GMT
  host: checkout.developers.ar.ua.la
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ual Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ualá, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ualá
provider_slug: ual
slug: ual-domain-security
source_filename: ual-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uala.com.ar\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 20:17:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.ualabis.com.ar\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 02:29:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: checkout.developers.ar.ua.la\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 20:17:19 2026 GMT\n  hsts: null\ndomains:\n- domain: uala.com.ar\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: ualabis.com.ar\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ual/refs/heads/main/security/ual-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Payments
- Banking
- Neobank
- Checkout
- Ecommerce
- Argentina
- Mexico
---
