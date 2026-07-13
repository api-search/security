---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: estuary.dev
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: run.app
  spf: true
hosts:
- cert_expires: Sep 10 23:09:48 2026 GMT
  host: estuary.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 02:44:19 2026 GMT
  host: docs.estuary.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:35:04 2026 GMT
  host: agent-api-1084703453822.us-central1.run.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Estuary Flow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Estuary Flow, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Estuary Flow
provider_slug: estuary-flow
slug: estuary-flow-domain-security
source_filename: estuary-flow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: estuary.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:09:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.estuary.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 02:44:19 2026 GMT\n  hsts: false\n- host: agent-api-1084703453822.us-central1.run.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:04 2026 GMT\n  hsts: null\ndomains:\n- domain: estuary.dev\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: run.app\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/estuary-flow/refs/heads/main/security/estuary-flow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data
- Streaming
- Change Data Capture
- CDC
- ETL
- ELT
- Real-Time
- Data Pipelines
- Connectors
- Lakehouse
---
