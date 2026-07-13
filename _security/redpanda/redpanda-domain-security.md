---
api_specs:
- filename: redpanda-admin-cluster-openapi.json
  format: json
  label: Redpanda Admin API
  slug: redpanda-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redpanda/refs/heads/main/openapi/redpanda-admin-cluster-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: redpanda.com
  spf: true
hosts:
- cert_expires: Sep 29 03:27:27 2026 GMT
  host: redpanda.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Redpanda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Redpanda, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Redpanda
provider_slug: redpanda
slug: redpanda-domain-security
source_filename: redpanda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: redpanda.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 03:27:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: redpanda.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/redpanda/refs/heads/main/security/redpanda-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Streaming
- Kafka
- Event Streaming
- Real-Time
- Data Platform
- Open Source
- C++
- Stream Processing
---
