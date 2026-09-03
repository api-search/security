---
api_specs:
- filename: tttech-nerve-management-system-openapi.yml
  format: yaml
  label: Nerve Management System API
  slug: nerve-management-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tttech/refs/heads/main/openapi/tttech-nerve-management-system-openapi.yml
- filename: tttech-nerve-node-openapi.yml
  format: yaml
  label: Nerve Node API
  slug: nerve-node-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tttech/refs/heads/main/openapi/tttech-nerve-node-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tttech.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: nerve.cloud
  spf: true
hosts:
- cert_expires: Oct 11 20:26:52 2026 GMT
  host: www.tttech.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: docs.nerve.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 18:49:52 2026 GMT
  host: trynerve1.nerve.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tttech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TTTech, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TTTech
provider_slug: tttech
slug: tttech-domain-security
source_filename: tttech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tttech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 20:26:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.nerve.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: trynerve1.nerve.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 18:49:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tttech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: nerve.cloud\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tttech/refs/heads/main/security/tttech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Industrial IoT
- Edge Computing
- Device Management
- Deterministic Networking
- Time-Sensitive Networking
- Industrial Automation
- Workload Orchestration
- Embedded Systems
- Safety Critical
- OPC UA
- MQTT
- CODESYS
- IEC 62443
---
