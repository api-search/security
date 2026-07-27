---
api_specs:
- filename: kore-wireless-connectivity-pro.yml
  format: yaml
  label: KORE Connectivity Pro API
  slug: kore-connectivity-pro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kore-wireless/refs/heads/main/openapi/kore-wireless-connectivity-pro.yml
- filename: kore-wireless-supersim.yml
  format: yaml
  label: KORE Super SIM API
  slug: kore-super-sim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kore-wireless/refs/heads/main/openapi/kore-wireless-supersim.yml
- filename: kore-wireless-programmable-wireless.yml
  format: yaml
  label: KORE Programmable Wireless API
  slug: kore-programmable-wireless-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kore-wireless/refs/heads/main/openapi/kore-wireless-programmable-wireless.yml
- filename: kore-wireless-sms.yml
  format: yaml
  label: KORE SMS API
  slug: kore-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kore-wireless/refs/heads/main/openapi/kore-wireless-sms.yml
- filename: kore-wireless-webhook.yml
  format: yaml
  label: KORE Webhook API
  slug: kore-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kore-wireless/refs/heads/main/openapi/kore-wireless-webhook.yml
- filename: kore-wireless-iam.yml
  format: yaml
  label: KORE Identity and Access Management API
  slug: kore-iam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kore-wireless/refs/heads/main/openapi/kore-wireless-iam.yml
- filename: kore-wireless-api-clients.yml
  format: yaml
  label: KORE API Clients API
  slug: kore-api-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kore-wireless/refs/heads/main/openapi/kore-wireless-api-clients.yml
- filename: kore-wireless-token.yml
  format: yaml
  label: KORE Token API
  slug: kore-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kore-wireless/refs/heads/main/openapi/kore-wireless-token.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: korewireless.com
  spf: true
hosts:
- cert_expires: Oct 22 22:19:25 2026 GMT
  host: www.korewireless.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 23:54:20 2026 GMT
  host: developer.korewireless.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 16:29:14 2026 GMT
  host: api.korewireless.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kore Wireless Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KORE Wireless, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: KORE Wireless
provider_slug: kore-wireless
slug: kore-wireless-domain-security
source_filename: kore-wireless-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.korewireless.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 22:19:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.korewireless.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:54:20 2026 GMT\n  hsts: false\n- host: api.korewireless.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 16:29:14 2026 GMT\n  hsts: null\ndomains:\n- domain: korewireless.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kore-wireless/refs/heads/main/security/kore-wireless-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Telecommunications
- United States
- IoT
- eSIM
- Connectivity
- MVNO
- SIM Management
- Roaming
- Messaging
- SMS
- Device Management
- Network APIs
---
