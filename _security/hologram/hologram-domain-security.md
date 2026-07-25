---
api_specs:
- filename: hologram-cellular-links-api-openapi.yml
  format: yaml
  label: Hologram Cellular Links API
  slug: hologram-cellular-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hologram/refs/heads/main/openapi/hologram-cellular-links-api-openapi.yml
- filename: hologram-devices-api-openapi.yml
  format: yaml
  label: Hologram Devices API
  slug: hologram-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hologram/refs/heads/main/openapi/hologram-devices-api-openapi.yml
- filename: hologram-messaging-api-openapi.yml
  format: yaml
  label: Hologram Messaging API
  slug: hologram-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hologram/refs/heads/main/openapi/hologram-messaging-api-openapi.yml
- filename: hologram-plans-api-openapi.yml
  format: yaml
  label: Hologram Plans API
  slug: hologram-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hologram/refs/heads/main/openapi/hologram-plans-api-openapi.yml
- filename: hologram-sms-api-openapi.yml
  format: yaml
  label: Hologram SMS API
  slug: hologram-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hologram/refs/heads/main/openapi/hologram-sms-api-openapi.yml
- filename: hologram-tags-api-openapi.yml
  format: yaml
  label: Hologram Tags API
  slug: hologram-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hologram/refs/heads/main/openapi/hologram-tags-api-openapi.yml
- filename: hologram-usage-api-openapi.yml
  format: yaml
  label: Hologram Usage API
  slug: hologram-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hologram/refs/heads/main/openapi/hologram-usage-api-openapi.yml
- filename: hologram-webhooks-api-openapi.yml
  format: yaml
  label: Hologram Webhooks API
  slug: hologram-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hologram/refs/heads/main/openapi/hologram-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hologram.io
  spf: true
hosts:
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: www.hologram.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 13:01:50 2026 GMT
  host: docs.hologram.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 23:59:59 2026 GMT
  host: dashboard.hologram.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hologram Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hologram, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hologram
provider_slug: hologram
slug: hologram-domain-security
source_filename: hologram-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hologram.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: false\n- host: docs.hologram.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 13:01:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: dashboard.hologram.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: hologram.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hologram/refs/heads/main/security/hologram-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- IoT
- Cellular
- Connectivity
- SIM
- M2M
---
