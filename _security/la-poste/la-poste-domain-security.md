---
api_specs:
- filename: swagger
  format: yaml
  label: La Poste Suivi (Tracking) API
  slug: la-poste-suivi-tracking-api
  spec_type: OpenAPI
  url: https://developer.laposte.fr/products/suivi/2/swagger
- filename: colissimo-shipping-openapi.json
  format: json
  label: La Poste Colissimo Shipping API
  slug: la-poste-colissimo-shipping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/la-poste/refs/heads/main/openapi/colissimo-shipping-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: laposte.fr
  spf: true
hosts:
- cert_expires: Nov 28 10:01:31 2026 GMT
  host: developer.laposte.fr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 28 10:01:31 2026 GMT
  host: api.laposte.fr
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 14:16:29 2026 GMT
  host: www.colissimo.entreprise.laposte.fr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: La Poste Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for La Poste, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: La Poste
provider_slug: la-poste
slug: la-poste-domain-security
source_filename: la-poste-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.laposte.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 10:01:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.laposte.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 10:01:31 2026 GMT\n  hsts: null\n- host: www.colissimo.entreprise.laposte.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 14:16:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: laposte.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/la-poste/refs/heads/main/security/la-poste-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Postal
- Parcel Tracking
- Address Validation
- Geolocation
- Shipping
- Open Data
- France
---
