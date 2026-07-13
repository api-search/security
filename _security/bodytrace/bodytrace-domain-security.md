---
api_specs:
- filename: bodytrace-openapi.yml
  format: yaml
  label: BodyTrace Observations (Data Values) API
  slug: bodytrace-observations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodytrace/refs/heads/main/openapi/bodytrace-openapi.yml
- filename: bodytrace-openapi.yml
  format: yaml
  label: BodyTrace Data Messages API
  slug: bodytrace-datamessages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodytrace/refs/heads/main/openapi/bodytrace-openapi.yml
- filename: bodytrace-openapi.yml
  format: yaml
  label: BodyTrace Devices API
  slug: bodytrace-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodytrace/refs/heads/main/openapi/bodytrace-openapi.yml
- filename: bodytrace-openapi.yml
  format: yaml
  label: BodyTrace Alerts API
  slug: bodytrace-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodytrace/refs/heads/main/openapi/bodytrace-openapi.yml
- filename: bodytrace-openapi.yml
  format: yaml
  label: BodyTrace Provisioning API
  slug: bodytrace-provisioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodytrace/refs/heads/main/openapi/bodytrace-openapi.yml
- filename: bodytrace-openapi.yml
  format: yaml
  label: BodyTrace Measurement Webhook (Push) API
  slug: bodytrace-measurement-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodytrace/refs/heads/main/openapi/bodytrace-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issuewild ";"
  - 0 issue "thawte.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: bodytrace.com
  spf: true
hosts:
- cert_expires: Aug 22 23:03:43 2026 GMT
  host: www.bodytrace.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: us.data.bodytrace.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: eu.data.bodytrace.com
  https: false
kind: domain-security
layout: security
method: probed
name: Bodytrace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BodyTrace, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: BodyTrace
provider_slug: bodytrace
slug: bodytrace-domain-security
source_filename: bodytrace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bodytrace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 23:03:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: us.data.bodytrace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: null\n- host: eu.data.bodytrace.com\n  https: false\ndomains:\n- domain: bodytrace.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \";\"\n  - 0 issue \"thawte.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bodytrace/refs/heads/main/security/bodytrace-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Remote Patient Monitoring
- RPM
- Cellular
- Medical Devices
- Digital Health
- Blood Pressure
- Connected Devices
- IoT
---
