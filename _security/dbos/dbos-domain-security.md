---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dbos.dev
  spf: true
hosts:
- cert_expires: Aug 17 21:14:28 2026 GMT
  host: www.dbos.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 13:40:49 2026 GMT
  host: docs.dbos.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dbos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DBOS, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: DBOS
provider_slug: dbos
slug: dbos-domain-security
source_filename: dbos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dbos.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 21:14:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.dbos.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 13:40:49 2026 GMT\n  hsts: false\ndomains:\n- domain: dbos.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dbos/refs/heads/main/security/dbos-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- API Composition
- Durable Execution
- Postgres
- Queues
- Scheduled Jobs
- Workflow
---
