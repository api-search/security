---
api_specs:
- filename: amazon-mediatailor-alerts-resourcearn-api-openapi.yml
  format: yaml
  label: Amazon MediaTailor Alerts#resourceArn API
  slug: amazon-mediatailor-alerts-resourcearn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/openapi/amazon-mediatailor-alerts-resourcearn-api-openapi.yml
- filename: amazon-mediatailor-channel-api-openapi.yml
  format: yaml
  label: Amazon MediaTailor Channel API
  slug: amazon-mediatailor-channel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/openapi/amazon-mediatailor-channel-api-openapi.yml
- filename: amazon-mediatailor-channels-api-openapi.yml
  format: yaml
  label: Amazon MediaTailor Channels API
  slug: amazon-mediatailor-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/openapi/amazon-mediatailor-channels-api-openapi.yml
- filename: amazon-mediatailor-configurelogs-api-openapi.yml
  format: yaml
  label: Amazon MediaTailor ConfigureLogs API
  slug: amazon-mediatailor-configurelogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/openapi/amazon-mediatailor-configurelogs-api-openapi.yml
- filename: amazon-mediatailor-playbackconfiguration-api-openapi.yml
  format: yaml
  label: Amazon MediaTailor PlaybackConfiguration API
  slug: amazon-mediatailor-playbackconfiguration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/openapi/amazon-mediatailor-playbackconfiguration-api-openapi.yml
- filename: amazon-mediatailor-playbackconfigurations-api-openapi.yml
  format: yaml
  label: Amazon MediaTailor PlaybackConfigurations API
  slug: amazon-mediatailor-playbackconfigurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/openapi/amazon-mediatailor-playbackconfigurations-api-openapi.yml
- filename: amazon-mediatailor-prefetchschedule-api-openapi.yml
  format: yaml
  label: Amazon MediaTailor PrefetchSchedule API
  slug: amazon-mediatailor-prefetchschedule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/openapi/amazon-mediatailor-prefetchschedule-api-openapi.yml
- filename: amazon-mediatailor-sourcelocation-api-openapi.yml
  format: yaml
  label: Amazon MediaTailor SourceLocation API
  slug: amazon-mediatailor-sourcelocation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/openapi/amazon-mediatailor-sourcelocation-api-openapi.yml
- filename: amazon-mediatailor-sourcelocations-api-openapi.yml
  format: yaml
  label: Amazon MediaTailor SourceLocations API
  slug: amazon-mediatailor-sourcelocations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/openapi/amazon-mediatailor-sourcelocations-api-openapi.yml
- filename: amazon-mediatailor-tags-api-openapi.yml
  format: yaml
  label: Amazon MediaTailor Tags API
  slug: amazon-mediatailor-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/openapi/amazon-mediatailor-tags-api-openapi.yml
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
kind: domain-security
layout: security
method: probed
name: Amazon Mediatailor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon MediaTailor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
slug: amazon-mediatailor-domain-security
source_filename: amazon-mediatailor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/security/amazon-mediatailor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Broadcasting
- Media Processing
- Media
---
