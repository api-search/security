---
api_specs:
- filename: truphone-openapi.yml
  format: yaml
  label: Truphone (1GLOBAL) SIMs / eSIMs API
  slug: truphone-sims-esims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truphone/refs/heads/main/openapi/truphone-openapi.yml
- filename: truphone-openapi.yml
  format: yaml
  label: Truphone (1GLOBAL) Connectivity / Usage API
  slug: truphone-connectivity-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truphone/refs/heads/main/openapi/truphone-openapi.yml
- filename: truphone-openapi.yml
  format: yaml
  label: Truphone (1GLOBAL) Plans API
  slug: truphone-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truphone/refs/heads/main/openapi/truphone-openapi.yml
- filename: truphone-openapi.yml
  format: yaml
  label: Truphone (1GLOBAL) Device Management API
  slug: truphone-device-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truphone/refs/heads/main/openapi/truphone-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 1global.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: truphone.com
  spf: true
hosts:
- cert_expires: Sep 13 12:13:50 2026 GMT
  host: www.1global.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 16:46:58 2026 GMT
  host: docs.things.1global.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 29 23:59:59 2026 GMT
  host: iot.truphone.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Truphone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Truphone (1GLOBAL), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Truphone (1GLOBAL)
provider_slug: truphone
slug: truphone-domain-security
source_filename: truphone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.1global.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 12:13:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.things.1global.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 16:46:58 2026 GMT\n  hsts: false\n- host: iot.truphone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 1global.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: truphone.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truphone/refs/heads/main/security/truphone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- eSIM
- IoT
- Connectivity
- SIM Management
- Telecom
- Mobile Network
---
