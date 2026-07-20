---
api_specs:
- filename: lisnr-tones-openapi-original.json
  format: json
  label: LISNR Tones Service API
  slug: tones-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lisnr/refs/heads/main/openapi/lisnr-tones-openapi-original.json
- filename: lisnr-portal-openapi-derived.json
  format: json
  label: LISNR Portal API
  slug: portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lisnr/refs/heads/main/openapi/lisnr-portal-openapi-derived.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lisnr.com
  spf: true
hosts:
- cert_expires: Sep 11 02:26:27 2026 GMT
  host: lisnr.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 23:59:59 2026 GMT
  host: portal.lisnr.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: tones.lisnr.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lisnr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LISNR, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LISNR
provider_slug: lisnr
slug: lisnr-domain-security
source_filename: lisnr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lisnr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 02:26:27 2026 GMT\n  hsts: false\n- host: portal.lisnr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 23:59:59 2026 GMT\n  hsts: false\n- host: tones.lisnr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: lisnr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lisnr/refs/heads/main/security/lisnr-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ultrasonic
- Data Over Audio
- Proximity
- Contactless Payments
- Device Pairing
- Identification
- Audio
- Internet of Things
- SDK
---
