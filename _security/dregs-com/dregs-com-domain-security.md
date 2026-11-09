---
api_specs:
- filename: dregs-com-badge-rules-api-openapi.yml
  format: yaml
  label: Dregs Badge Rules API
  slug: dregs-com-badge-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dregs-com/openapi/dregs-com-badge-rules-api-openapi.yml
- filename: dregs-com-channels-api-openapi.yml
  format: yaml
  label: Dregs Channels API
  slug: dregs-com-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dregs-com/openapi/dregs-com-channels-api-openapi.yml
- filename: dregs-com-dashboard-api-openapi.yml
  format: yaml
  label: Dregs Dashboard API
  slug: dregs-com-dashboard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dregs-com/openapi/dregs-com-dashboard-api-openapi.yml
- filename: dregs-com-datasets-api-openapi.yml
  format: yaml
  label: Dregs Datasets API
  slug: dregs-com-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dregs-com/openapi/dregs-com-datasets-api-openapi.yml
- filename: dregs-com-devices-api-openapi.yml
  format: yaml
  label: Dregs Devices API
  slug: dregs-com-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dregs-com/openapi/dregs-com-devices-api-openapi.yml
- filename: dregs-com-escalation-rules-api-openapi.yml
  format: yaml
  label: Dregs Escalation Rules API
  slug: dregs-com-escalation-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dregs-com/openapi/dregs-com-escalation-rules-api-openapi.yml
- filename: dregs-com-escalations-api-openapi.yml
  format: yaml
  label: Dregs Escalations API
  slug: dregs-com-escalations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dregs-com/openapi/dregs-com-escalations-api-openapi.yml
- filename: dregs-com-events-api-openapi.yml
  format: yaml
  label: Dregs Events API
  slug: dregs-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dregs-com/openapi/dregs-com-events-api-openapi.yml
- filename: dregs-com-groups-api-openapi.yml
  format: yaml
  label: Dregs Groups API
  slug: dregs-com-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dregs-com/openapi/dregs-com-groups-api-openapi.yml
- filename: dregs-com-identities-api-openapi.yml
  format: yaml
  label: Dregs Identities API
  slug: dregs-com-identities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dregs-com/openapi/dregs-com-identities-api-openapi.yml
- filename: dregs-com-mappings-api-openapi.yml
  format: yaml
  label: Dregs Mappings API
  slug: dregs-com-mappings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dregs-com/openapi/dregs-com-mappings-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dregs.com
  spf: true
hosts:
- cert_expires: Apr 20 23:59:59 2027 GMT
  host: dregs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dregs Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dregs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dregs
provider_slug: dregs-com
slug: dregs-com-domain-security
source_filename: dregs-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dregs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dregs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dregs-com/security/dregs-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fraud Prevention
- Abuse Prevention
- Identity Scoring
- Bot Detection
- Account Verification
---
