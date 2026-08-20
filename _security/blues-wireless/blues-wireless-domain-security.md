---
api_specs:
- filename: blues-wireless-alert-api-openapi.yml
  format: yaml
  label: Blues alert API
  slug: blues-wireless-alert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blues-wireless/refs/heads/main/openapi/blues-wireless-alert-api-openapi.yml
- filename: blues-wireless-authorization-api-openapi.yml
  format: yaml
  label: Blues authorization API
  slug: blues-wireless-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blues-wireless/refs/heads/main/openapi/blues-wireless-authorization-api-openapi.yml
- filename: blues-wireless-billing-account-api-openapi.yml
  format: yaml
  label: Blues billing_account API
  slug: blues-wireless-billing-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blues-wireless/refs/heads/main/openapi/blues-wireless-billing-account-api-openapi.yml
- filename: blues-wireless-device-api-openapi.yml
  format: yaml
  label: Blues device API
  slug: blues-wireless-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blues-wireless/refs/heads/main/openapi/blues-wireless-device-api-openapi.yml
- filename: blues-wireless-event-api-openapi.yml
  format: yaml
  label: Blues event API
  slug: blues-wireless-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blues-wireless/refs/heads/main/openapi/blues-wireless-event-api-openapi.yml
- filename: blues-wireless-external-devices-api-openapi.yml
  format: yaml
  label: Blues external devices API
  slug: blues-wireless-external-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blues-wireless/refs/heads/main/openapi/blues-wireless-external-devices-api-openapi.yml
- filename: blues-wireless-jobs-api-openapi.yml
  format: yaml
  label: Blues jobs API
  slug: blues-wireless-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blues-wireless/refs/heads/main/openapi/blues-wireless-jobs-api-openapi.yml
- filename: blues-wireless-monitor-api-openapi.yml
  format: yaml
  label: Blues monitor API
  slug: blues-wireless-monitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blues-wireless/refs/heads/main/openapi/blues-wireless-monitor-api-openapi.yml
- filename: blues-wireless-organization-api-openapi.yml
  format: yaml
  label: Blues organization API
  slug: blues-wireless-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blues-wireless/refs/heads/main/openapi/blues-wireless-organization-api-openapi.yml
- filename: blues-wireless-project-api-openapi.yml
  format: yaml
  label: Blues project API
  slug: blues-wireless-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blues-wireless/refs/heads/main/openapi/blues-wireless-project-api-openapi.yml
- filename: blues-wireless-route-api-openapi.yml
  format: yaml
  label: Blues route API
  slug: blues-wireless-route-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blues-wireless/refs/heads/main/openapi/blues-wireless-route-api-openapi.yml
- filename: blues-wireless-usage-api-openapi.yml
  format: yaml
  label: Blues usage API
  slug: blues-wireless-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blues-wireless/refs/heads/main/openapi/blues-wireless-usage-api-openapi.yml
- filename: blues-wireless-webhook-api-openapi.yml
  format: yaml
  label: Blues webhook API
  slug: blues-wireless-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blues-wireless/refs/heads/main/openapi/blues-wireless-webhook-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: blues.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: blues.io
  spf: true
hosts:
- cert_expires: Aug 19 14:56:10 2026 GMT
  host: blues.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: dev.blues.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: api.notefile.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blues Wireless Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blues, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Blues
provider_slug: blues-wireless
slug: blues-wireless-domain-security
source_filename: blues-wireless-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blues.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 14:56:10 2026 GMT\n  hsts: false\n- host: dev.blues.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: false\n- host: api.notefile.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: blues.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: blues.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blues-wireless/refs/heads/main/security/blues-wireless-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- IoT
- Cellular
- Connectivity
- Device Management
- Fleet Management
- Satellite
- LoRA
- Wi-Fi
- Notecard
- Notehub
---
