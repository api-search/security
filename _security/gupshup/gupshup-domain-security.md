---
api_specs:
- filename: gupshup-openapi.yml
  format: yaml
  label: Gupshup WhatsApp Messaging API
  slug: gupshup-whatsapp-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gupshup/refs/heads/main/openapi/gupshup-openapi.yml
- filename: gupshup-openapi.yml
  format: yaml
  label: Gupshup WhatsApp Template Messaging API
  slug: gupshup-whatsapp-template-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gupshup/refs/heads/main/openapi/gupshup-openapi.yml
- filename: gupshup-openapi.yml
  format: yaml
  label: Gupshup WhatsApp Opt-In Management API
  slug: gupshup-whatsapp-optin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gupshup/refs/heads/main/openapi/gupshup-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gupshup.io
  spf: true
  spf_policy: ~all
hosts:
- cert_expires: Feb 11 23:59:59 2027 GMT
  cert_issuer: Amazon RSA 2048 M01
  host: api.gupshup.io
  hsts: false
  https: true
  notes: WhatsApp / messaging API host. Fronted by an AWS ALB in ap-south-1 (India). Root path returns 404; API paths are under /wa and /sm.
  server: GupShup-Webserver
  tls_version: TLSv1.3
- cert_expires: Mar 11 23:59:59 2027 GMT
  cert_issuer: Amazon RSA 2048 M04
  host: partner.gupshup.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  server: AmazonS3
  tls_version: TLSv1.3
- cert_expires: Sep  8 23:56:53 2026 GMT
  cert_issuer: Let's Encrypt
  host: docs.gupshup.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  server: cloudflare
  tls_version: TLSv1.3
- cert_expires: Oct 19 23:59:59 2026 GMT
  cert_issuer: Thawte TLS RSA CA G1 (DigiCert)
  host: gupshup.io
  hsts: false
  https: true
  server: awselb/2.0
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gupshup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gupshup, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Gupshup
provider_slug: gupshup
slug: gupshup-domain-security
source_filename: gupshup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.gupshup.io\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Amazon RSA 2048 M01\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: false\n  server: GupShup-Webserver\n  notes: WhatsApp / messaging API host. Fronted by an AWS ALB in ap-south-1 (India). Root path returns 404; API paths are under /wa and /sm.\n- host: partner.gupshup.io\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Amazon RSA 2048 M04\n  cert_expires: Mar 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  server: AmazonS3\n- host: docs.gupshup.io\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Let's Encrypt\n  cert_expires: Sep  8 23:56:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  server: cloudflare\n- host: gupshup.io\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Thawte TLS RSA CA G1 (DigiCert)\n  cert_expires: Oct 19 23:59:59 2026 GMT\n\
  \  hsts: false\n  server: awselb/2.0\ndomains:\n- domain: gupshup.io\n  dnssec: false\n  caa: []\n  spf: true\n  spf_policy: ~all\n  dmarc: true\n  dmarc_policy: reject\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gupshup/refs/heads/main/security/gupshup-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Messaging
- WhatsApp
- Conversational AI
- CPaaS
- SMS
- RCS
- India
- Chatbots
- Business Messaging
- Communications
---
