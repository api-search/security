---
api_specs:
- filename: schlage-home-openapi.yml
  format: yaml
  label: Schlage Home API
  slug: schlage-home-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allegion/refs/heads/main/openapi/schlage-home-openapi.yml
- filename: engage-credentialing-openapi.yml
  format: yaml
  label: ENGAGE Cloud Credentialing API
  slug: engage-credentialing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allegion/refs/heads/main/openapi/engage-credentialing-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: allegion.com
  spf: true
hosts:
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: developerapi.allegion.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 23 21:26:32 2026 GMT
  host: developer.allegion.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: api.allegion.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Allegion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Allegion, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Allegion
provider_slug: allegion
slug: allegion-domain-security
source_filename: allegion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developerapi.allegion.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.allegion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 21:26:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.allegion.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: allegion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allegion/refs/heads/main/security/allegion-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Access Control
- Smart Lock
- Smart Home
- Mobile Credentials
- Bluetooth
- BLE
- IoT
- Security
- Webhooks
- OAuth
- Schlage
- Von Duprin
- ENGAGE
---
