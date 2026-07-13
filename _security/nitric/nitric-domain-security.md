---
api_specs:
- filename: nitric-openapi.yml
  format: yaml
  label: Nitric API Resource
  slug: nitric-api-resource
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nitric/refs/heads/main/openapi/nitric-openapi.yml
- filename: nitric-openapi.yml
  format: yaml
  label: Nitric Schedule Resource
  slug: nitric-schedule-resource
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nitric/refs/heads/main/openapi/nitric-openapi.yml
- filename: nitric-openapi.yml
  format: yaml
  label: Nitric Queue Resource
  slug: nitric-queue-resource
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nitric/refs/heads/main/openapi/nitric-openapi.yml
- filename: nitric-openapi.yml
  format: yaml
  label: Nitric Topic Resource
  slug: nitric-topic-resource
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nitric/refs/heads/main/openapi/nitric-openapi.yml
- filename: nitric-openapi.yml
  format: yaml
  label: Nitric Bucket Resource
  slug: nitric-bucket-resource
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nitric/refs/heads/main/openapi/nitric-openapi.yml
- filename: nitric-openapi.yml
  format: yaml
  label: Nitric Key-Value Resource
  slug: nitric-keyvalue-resource
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nitric/refs/heads/main/openapi/nitric-openapi.yml
- filename: nitric-openapi.yml
  format: yaml
  label: Nitric Secret Resource
  slug: nitric-secret-resource
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nitric/refs/heads/main/openapi/nitric-openapi.yml
- filename: nitric-openapi.yml
  format: yaml
  label: Nitric Websocket Resource
  slug: nitric-websocket-resource
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nitric/refs/heads/main/openapi/nitric-openapi.yml
- filename: nitric-openapi.yml
  format: yaml
  label: Nitric SQL Database Resource
  slug: nitric-sql-resource
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nitric/refs/heads/main/openapi/nitric-openapi.yml
- filename: nitric-openapi.yml
  format: yaml
  label: Nitric CLI
  slug: nitric-cli
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nitric/refs/heads/main/openapi/nitric-openapi.yml
- filename: nitric-openapi.yml
  format: yaml
  label: Nitric Provider Plugins
  slug: nitric-provider-plugins
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nitric/refs/heads/main/openapi/nitric-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nitric.io
  spf: true
hosts:
- cert_expires: Sep 14 02:13:32 2026 GMT
  host: nitric.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nitric Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nitric, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nitric
provider_slug: nitric
slug: nitric-domain-security
source_filename: nitric-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nitric.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 02:13:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nitric.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nitric/refs/heads/main/security/nitric-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Infrastructure from Code
- Cloud Framework
- SDK
- CLI
- Serverless
- Multi-Cloud
---
