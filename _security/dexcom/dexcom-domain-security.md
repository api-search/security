---
api_specs:
- filename: dexcom-alerts-api-openapi.yml
  format: yaml
  label: Dexcom Alerts API
  slug: dexcom-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dexcom/refs/heads/main/openapi/dexcom-alerts-api-openapi.yml
- filename: dexcom-authentication-api-openapi.yml
  format: yaml
  label: Dexcom Authentication API
  slug: dexcom-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dexcom/refs/heads/main/openapi/dexcom-authentication-api-openapi.yml
- filename: dexcom-calibrations-api-openapi.yml
  format: yaml
  label: Dexcom Calibrations API
  slug: dexcom-calibrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dexcom/refs/heads/main/openapi/dexcom-calibrations-api-openapi.yml
- filename: dexcom-data-range-api-openapi.yml
  format: yaml
  label: Dexcom Data Range API
  slug: dexcom-data-range-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dexcom/refs/heads/main/openapi/dexcom-data-range-api-openapi.yml
- filename: dexcom-devices-api-openapi.yml
  format: yaml
  label: Dexcom Devices API
  slug: dexcom-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dexcom/refs/heads/main/openapi/dexcom-devices-api-openapi.yml
- filename: dexcom-estimated-glucose-values-api-openapi.yml
  format: yaml
  label: Dexcom Estimated Glucose Values API
  slug: dexcom-estimated-glucose-values-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dexcom/refs/heads/main/openapi/dexcom-estimated-glucose-values-api-openapi.yml
- filename: dexcom-events-api-openapi.yml
  format: yaml
  label: Dexcom Events API
  slug: dexcom-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dexcom/refs/heads/main/openapi/dexcom-events-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dexcom.com
  spf: true
hosts:
- cert_expires: Aug 14 03:00:38 2026 GMT
  host: www.dexcom.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 05:39:46 2026 GMT
  host: developer.dexcom.com
  hsts: true
  hsts_max_age: 15780000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 05:33:10 2026 GMT
  host: api.dexcom.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dexcom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dexcom, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Dexcom
provider_slug: dexcom
slug: dexcom-domain-security
source_filename: dexcom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dexcom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 03:00:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.dexcom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 05:39:46 2026 GMT\n  hsts: true\n  hsts_max_age: 15780000\n- host: api.dexcom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 05:33:10 2026 GMT\n  hsts: null\ndomains:\n- domain: dexcom.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dexcom/refs/heads/main/security/dexcom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Continuous Glucose Monitoring
- Diabetes
- Digital Health
- Glucose
- Healthcare
- Medical Devices
- Wearables
---
