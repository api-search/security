---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: superduper.io
  spf: true
hosts:
- cert_expires: Oct 26 23:59:59 2026 GMT
  host: superduper.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 01:41:16 2026 GMT
  host: docs.superduper.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Superduperdb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Superduper, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Superduper
provider_slug: superduperdb
slug: superduperdb-domain-security
source_filename: superduperdb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: superduper.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 23:59:59 2026 GMT\n  hsts: false\n- host: docs.superduper.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 01:41:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: superduper.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superduperdb/refs/heads/main/security/superduperdb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Framework
- Vector Search
- RAG
- LLMs
- MLOps
- Open Source
- AI Agents
---
