---
api_specs:
- filename: infobip-ai-hub-api-openapi.yml
  format: yaml
  label: Infobip AI Hub API
  slug: infobip-ai-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infobip/refs/heads/main/openapi/infobip-ai-hub-api-openapi.yml
- filename: infobip-channels-api-openapi.yml
  format: yaml
  label: Infobip Channels API
  slug: infobip-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infobip/refs/heads/main/openapi/infobip-channels-api-openapi.yml
- filename: infobip-connectivity-api-openapi.yml
  format: yaml
  label: Infobip Connectivity API
  slug: infobip-connectivity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infobip/refs/heads/main/openapi/infobip-connectivity-api-openapi.yml
- filename: infobip-customer-engagement-api-openapi.yml
  format: yaml
  label: Infobip Customer Engagement API
  slug: infobip-customer-engagement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infobip/refs/heads/main/openapi/infobip-customer-engagement-api-openapi.yml
- filename: infobip-platform-api-openapi.yml
  format: yaml
  label: Infobip Platform API
  slug: infobip-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infobip/refs/heads/main/openapi/infobip-platform-api-openapi.yml
- filename: infobip-tools-api-openapi.yml
  format: yaml
  label: Infobip Tools API
  slug: infobip-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infobip/refs/heads/main/openapi/infobip-tools-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: infobip.com
  spf: true
hosts:
- cert_expires: Sep 11 04:29:35 2026 GMT
  host: www.infobip.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 23 23:59:59 2026 GMT
  host: api.infobip.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Infobip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Infobip, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Infobip
provider_slug: infobip
slug: infobip-domain-security
source_filename: infobip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.infobip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 04:29:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.infobip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: infobip.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infobip/refs/heads/main/security/infobip-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Telecommunications
- Croatia
- CPaaS
- Messaging
- SMS
- Voice
- RCS
- WhatsApp
- Email
- Network APIs
- CAMARA
- Open Gateway
- Identity Verification
- SIM Swap
- Number Verification
- Omnichannel
- Aggregator
- Customer Engagement
---
