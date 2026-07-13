---
api_specs:
- filename: quix-openapi.yml
  format: yaml
  label: Quix Streaming Writer API
  slug: streaming-writer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quix/refs/heads/main/openapi/quix-openapi.yml
- filename: quix-asyncapi.yml
  format: yaml
  label: Quix Streaming Reader API (Real-time)
  slug: streaming-reader-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/quix/refs/heads/main/asyncapi/quix-asyncapi.yml
- filename: quix-openapi.yml
  format: yaml
  label: Quix Portal API (Management)
  slug: portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quix/refs/heads/main/openapi/quix-openapi.yml
- filename: quix-openapi.yml
  format: yaml
  label: Quix Topics & Deployments API
  slug: topics-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quix/refs/heads/main/openapi/quix-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: quix.io
  spf: true
hosts:
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: quix.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: portal-api.platform.quix.io
  https: false
kind: domain-security
layout: security
method: probed
name: Quix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quix, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Quix
provider_slug: quix
slug: quix-domain-security
source_filename: quix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quix.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: false\n- host: portal-api.platform.quix.io\n  https: false\ndomains:\n- domain: quix.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quix/refs/heads/main/security/quix-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Stream Processing
- Real Time
- Kafka
- Python
- Streaming Data
---
