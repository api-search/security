---
api_specs:
- filename: bodyspec-api-status-api-openapi.yml
  format: yaml
  label: BodySpec API Status API
  slug: bodyspec-api-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-api-status-api-openapi.yml
- filename: bodyspec-appointments-api-openapi.yml
  format: yaml
  label: BodySpec Appointments API
  slug: bodyspec-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-appointments-api-openapi.yml
- filename: bodyspec-availability-api-openapi.yml
  format: yaml
  label: BodySpec Availability API
  slug: bodyspec-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-availability-api-openapi.yml
- filename: bodyspec-bodyspec-api-api-openapi.yml
  format: yaml
  label: BodySpec BodySpec API
  slug: bodyspec-bodyspec-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-bodyspec-api-api-openapi.yml
- filename: bodyspec-locations-api-openapi.yml
  format: yaml
  label: BodySpec Locations API
  slug: bodyspec-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-locations-api-openapi.yml
- filename: bodyspec-partner-appointments-api-openapi.yml
  format: yaml
  label: BodySpec Partner Appointments API
  slug: bodyspec-partner-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-partner-appointments-api-openapi.yml
- filename: bodyspec-partner-intake-api-openapi.yml
  format: yaml
  label: BodySpec Partner Intake API
  slug: bodyspec-partner-intake-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-partner-intake-api-openapi.yml
- filename: bodyspec-partner-orders-api-openapi.yml
  format: yaml
  label: BodySpec Partner Orders API
  slug: bodyspec-partner-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-partner-orders-api-openapi.yml
- filename: bodyspec-partner-results-api-openapi.yml
  format: yaml
  label: BodySpec Partner Results API
  slug: bodyspec-partner-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-partner-results-api-openapi.yml
- filename: bodyspec-partner-users-api-openapi.yml
  format: yaml
  label: BodySpec Partner Users API
  slug: bodyspec-partner-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-partner-users-api-openapi.yml
- filename: bodyspec-partner-webhooks-api-openapi.yml
  format: yaml
  label: BodySpec Partner Webhooks API
  slug: bodyspec-partner-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-partner-webhooks-api-openapi.yml
- filename: bodyspec-reservations-api-openapi.yml
  format: yaml
  label: BodySpec Reservations API
  slug: bodyspec-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-reservations-api-openapi.yml
- filename: bodyspec-results-api-openapi.yml
  format: yaml
  label: BodySpec Results API
  slug: bodyspec-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-results-api-openapi.yml
- filename: bodyspec-services-api-openapi.yml
  format: yaml
  label: BodySpec Services API
  slug: bodyspec-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-services-api-openapi.yml
- filename: bodyspec-users-api-openapi.yml
  format: yaml
  label: BodySpec Users API
  slug: bodyspec-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bodyspec.com
  spf: true
hosts:
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: www.bodyspec.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bodyspec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BodySpec, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BodySpec
provider_slug: bodyspec
slug: bodyspec-domain-security
source_filename: bodyspec-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bodyspec.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: bodyspec.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/security/bodyspec-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Health
- Fitness
- Data
---
