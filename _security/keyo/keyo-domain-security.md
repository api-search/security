---
api_specs:
- filename: keyo-openapi.yml
  format: yaml
  label: Keyo REST API
  slug: keyo-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keyo/refs/heads/main/openapi/keyo-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: keyo.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: keyo.co
  spf: true
hosts:
- cert_expires: Sep 14 15:56:05 2026 GMT
  host: keyo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 18:31:39 2026 GMT
  host: api.keyo.co
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 18:31:39 2026 GMT
  host: api.africa.keyo.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Keyo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Keyo, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Keyo
provider_slug: keyo
slug: keyo-domain-security
source_filename: keyo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: keyo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 15:56:05 2026 GMT\n  hsts: false\n- host: api.keyo.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 18:31:39 2026 GMT\n  hsts: null\n- host: api.africa.keyo.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 18:31:39 2026 GMT\n  hsts: null\ndomains:\n- domain: keyo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: keyo.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keyo/refs/heads/main/security/keyo-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Biometrics
- Identity
- Authentication
- Palm Recognition
- Access Control
- Payments
- Identity Verification
---
