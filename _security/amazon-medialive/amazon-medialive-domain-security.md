---
api_specs:
- filename: amazon-medialive-prod-api-openapi.yml
  format: yaml
  label: Amazon MediaLive Prod API
  slug: amazon-medialive-prod-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-medialive/openapi/amazon-medialive-prod-api-openapi.yml
- filename: amazon-medialive-alerts-api-openapi.yml
  format: yaml
  label: Amazon MediaLive Medialive Alerts API
  slug: amazon-medialive-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-medialive/openapi/amazon-medialive-alerts-api-openapi.yml
- filename: amazon-medialive-channelplacementgroups-api-openapi.yml
  format: yaml
  label: Amazon MediaLive Medialive Channelplacementgroups API
  slug: amazon-medialive-channelplacementgroups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-medialive/openapi/amazon-medialive-channelplacementgroups-api-openapi.yml
- filename: amazon-medialive-nodes-api-openapi.yml
  format: yaml
  label: Amazon MediaLive Medialive Nodes API
  slug: amazon-medialive-nodes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-medialive/openapi/amazon-medialive-nodes-api-openapi.yml
- filename: amazon-medialive-operations-api-openapi.yml
  format: yaml
  label: Amazon MediaLive Medialive Operations API
  slug: amazon-medialive-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-medialive/openapi/amazon-medialive-operations-api-openapi.yml
- filename: amazon-medialive-programs-api-openapi.yml
  format: yaml
  label: Amazon MediaLive Medialive Programs API
  slug: amazon-medialive-programs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-medialive/openapi/amazon-medialive-programs-api-openapi.yml
- filename: amazon-medialive-schedule-api-openapi.yml
  format: yaml
  label: Amazon MediaLive Medialive Schedule API
  slug: amazon-medialive-schedule-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-medialive/openapi/amazon-medialive-schedule-api-openapi.yml
- filename: amazon-medialive-start-api-openapi.yml
  format: yaml
  label: Amazon MediaLive Medialive Start API
  slug: amazon-medialive-start-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-medialive/openapi/amazon-medialive-start-api-openapi.yml
- filename: amazon-medialive-stop-api-openapi.yml
  format: yaml
  label: Amazon MediaLive Medialive Stop API
  slug: amazon-medialive-stop-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-medialive/openapi/amazon-medialive-stop-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Amazon Medialive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon MediaLive, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
slug: amazon-medialive-domain-security
source_filename: amazon-medialive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/amazon-medialive/security/amazon-medialive-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Broadcasting
- Media Processing
- Media
---
