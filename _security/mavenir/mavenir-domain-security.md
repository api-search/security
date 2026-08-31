---
api_specs:
- filename: mavenir-onetoonecall-api-openapi.yml
  format: yaml
  label: Mavenir One To One Call API
  slug: mavenir-onetoonecall-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mavenir/refs/heads/main/openapi/mavenir-onetoonecall-api-openapi.yml
- filename: mavenir-push-token-api-openapi.yml
  format: yaml
  label: Mavenir Push Token API
  slug: mavenir-push-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mavenir/refs/heads/main/openapi/mavenir-push-token-api-openapi.yml
- filename: mavenir-racm-api-openapi.yml
  format: yaml
  label: Mavenir RACM API
  slug: mavenir-racm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mavenir/refs/heads/main/openapi/mavenir-racm-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: mavenir.com
  spf: true
hosts:
- cert_expires: Sep 30 21:42:20 2026 GMT
  host: www.mavenir.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mavenir Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mavenir, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Mavenir
provider_slug: mavenir
slug: mavenir-domain-security
source_filename: mavenir-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mavenir.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 21:42:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mavenir.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mavenir/refs/heads/main/security/mavenir-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Telecommunications
- United States
- Network Vendor
- Network APIs
- CAMARA
- Open Gateway
- BSS
- OSS
- TM Forum
- Open RAN
- 5G
- IMS
- Messaging
- Network Exposure Function
- Standards
---
