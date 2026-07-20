---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kosmoslabs.ai
  spf: true
hosts:
- cert_expires: Sep 10 01:21:57 2026 GMT
  host: kosmoslabs.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 01:11:44 2026 GMT
  host: docs.kosmoslabs.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 08:06:08 2026 GMT
  host: ingest.kosmoslabs.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kosmoslabs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kosmos AI Labs, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kosmos AI Labs
provider_slug: kosmoslabs
slug: kosmoslabs-domain-security
source_filename: kosmoslabs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kosmoslabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 01:21:57 2026 GMT\n  hsts: false\n- host: docs.kosmoslabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 01:11:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ingest.kosmoslabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 08:06:08 2026 GMT\n  hsts: null\ndomains:\n- domain: kosmoslabs.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kosmoslabs/refs/heads/main/security/kosmoslabs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Operational Intelligence
- Observability
- OpenTelemetry
- Incident Management
- Root Cause Analysis
- AIOps
- Enterprise Software
---
