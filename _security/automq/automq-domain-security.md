---
api_specs:
- filename: automq-ai-info-api-openapi.yml
  format: yaml
  label: AutoMQ Ai Info API
  slug: automq-ai-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automq/refs/heads/main/openapi/automq-ai-info-api-openapi.yml
- filename: automq-llms-full-txt-api-openapi.yml
  format: yaml
  label: AutoMQ Llms Full.txt API
  slug: automq-llms-full-txt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automq/refs/heads/main/openapi/automq-llms-full-txt-api-openapi.yml
- filename: automq-llms-txt-api-openapi.yml
  format: yaml
  label: AutoMQ Llms.txt API
  slug: automq-llms-txt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automq/refs/heads/main/openapi/automq-llms-txt-api-openapi.yml
- filename: automq-robots-txt-api-openapi.yml
  format: yaml
  label: AutoMQ Robots.txt API
  slug: automq-robots-txt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automq/refs/heads/main/openapi/automq-robots-txt-api-openapi.yml
- filename: automq-well-known-api-openapi.yml
  format: yaml
  label: AutoMQ .well Known API
  slug: automq-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automq/refs/heads/main/openapi/automq-well-known-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: automq.com
  spf: true
hosts:
- cert_expires: Dec 27 18:05:37 2026 GMT
  host: www.automq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Automq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AutoMQ, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AutoMQ
provider_slug: automq
slug: automq-domain-security
source_filename: automq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.automq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 18:05:37 2026 GMT\n  hsts: false\ndomains:\n- domain: automq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/automq/refs/heads/main/security/automq-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Kafka
- Streaming
- Event Streaming
- Object Storage
- Open Source
- Cloud
---
