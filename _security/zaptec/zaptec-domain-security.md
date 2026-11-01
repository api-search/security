---
api_specs:
- filename: zaptec-chargehistory-api-openapi.yml
  format: yaml
  label: Zaptec Charge History API
  slug: zaptec-chargehistory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zaptec/openapi/zaptec-chargehistory-api-openapi.yml
- filename: zaptec-charger-api-openapi.yml
  format: yaml
  label: Zaptec Charger API
  slug: zaptec-charger-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zaptec/openapi/zaptec-charger-api-openapi.yml
- filename: zaptec-chargerfirmware-api-openapi.yml
  format: yaml
  label: Zaptec Charger Firmware API
  slug: zaptec-chargerfirmware-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zaptec/openapi/zaptec-chargerfirmware-api-openapi.yml
- filename: zaptec-constants-api-openapi.yml
  format: yaml
  label: Zaptec Constants API
  slug: zaptec-constants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zaptec/openapi/zaptec-constants-api-openapi.yml
- filename: zaptec-installation-api-openapi.yml
  format: yaml
  label: Zaptec Installation API
  slug: zaptec-installation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zaptec/openapi/zaptec-installation-api-openapi.yml
- filename: zaptec-session-api-openapi.yml
  format: yaml
  label: Zaptec Session API
  slug: zaptec-session-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zaptec/openapi/zaptec-session-api-openapi.yml
- filename: zaptec-user-group-api-openapi.yml
  format: yaml
  label: Zaptec User Group API
  slug: zaptec-user-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zaptec/openapi/zaptec-user-group-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: zaptec.com
  spf: true
hosts:
- cert_expires: Dec 11 13:19:01 2026 GMT
  host: zaptec.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Zaptec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zaptec, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Zaptec
provider_slug: zaptec
slug: zaptec-domain-security
source_filename: zaptec-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zaptec.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 13:19:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: zaptec.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/zaptec/security/zaptec-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- EVCharging
- SmartCharging
- Energy
- Sustainability
- Platform
---
