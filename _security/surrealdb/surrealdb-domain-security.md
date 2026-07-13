---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "cloudflare.org"
  - 0 issue "letsencrypt.org"
  - 0 issue "letsencrypt.org;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/54403714"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: surrealdb.com
  spf: true
hosts:
- cert_expires: Aug 21 20:41:54 2026 GMT
  host: surrealdb.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: cloud.surrealdb.com
  https: false
kind: domain-security
layout: security
method: probed
name: Surrealdb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SurrealDB, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SurrealDB
provider_slug: surrealdb
slug: surrealdb-domain-security
source_filename: surrealdb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: surrealdb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 20:41:54 2026 GMT\n  hsts: null\n- host: cloud.surrealdb.com\n  https: false\ndomains:\n- domain: surrealdb.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"cloudflare.org\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/54403714\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/surrealdb/refs/heads/main/security/surrealdb-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Database
- Multi-Model
- Graph Database
- Document Database
- Vector Database
- Time-Series
- SurrealQL
- AI
- MCP
---
