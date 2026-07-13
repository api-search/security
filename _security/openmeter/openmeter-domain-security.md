---
api_specs:
- filename: openmeter-openapi.yml
  format: yaml
  label: OpenMeter Events Ingestion API
  slug: openmeter-events-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmeter/refs/heads/main/openapi/openmeter-openapi.yml
- filename: openmeter-openapi.yml
  format: yaml
  label: OpenMeter Meters API
  slug: openmeter-meters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmeter/refs/heads/main/openapi/openmeter-openapi.yml
- filename: openmeter-openapi.yml
  format: yaml
  label: OpenMeter Usage Query API
  slug: openmeter-usage-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmeter/refs/heads/main/openapi/openmeter-openapi.yml
- filename: openmeter-openapi.yml
  format: yaml
  label: OpenMeter Subjects API
  slug: openmeter-subjects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmeter/refs/heads/main/openapi/openmeter-openapi.yml
- filename: openmeter-openapi.yml
  format: yaml
  label: OpenMeter Entitlements API
  slug: openmeter-entitlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmeter/refs/heads/main/openapi/openmeter-openapi.yml
- filename: openmeter-openapi.yml
  format: yaml
  label: OpenMeter Features API
  slug: openmeter-features-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmeter/refs/heads/main/openapi/openmeter-openapi.yml
- filename: openmeter-openapi.yml
  format: yaml
  label: OpenMeter Grants API
  slug: openmeter-grants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmeter/refs/heads/main/openapi/openmeter-openapi.yml
- filename: openmeter-openapi.yml
  format: yaml
  label: OpenMeter Notifications API
  slug: openmeter-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmeter/refs/heads/main/openapi/openmeter-openapi.yml
- filename: openmeter-openapi.yml
  format: yaml
  label: OpenMeter Billing and Plans API
  slug: openmeter-billing-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmeter/refs/heads/main/openapi/openmeter-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: openmeter.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: openmeter.cloud
  spf: true
hosts:
- cert_expires: Sep 30 05:58:39 2026 GMT
  host: openmeter.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 04:23:31 2026 GMT
  host: openmeter.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openmeter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenMeter, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: OpenMeter
provider_slug: openmeter
slug: openmeter-domain-security
source_filename: openmeter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openmeter.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 05:58:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: openmeter.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 04:23:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: openmeter.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: openmeter.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openmeter/refs/heads/main/security/openmeter-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Usage Metering
- Billing
- Entitlements
- CloudEvents
- Open Source
- AI
---
