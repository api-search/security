---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: postgresml.org
  spf: false
hosts:
- cert_expires: Sep 21 10:13:20 2026 GMT
  host: postgresml.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Postgresml Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PostgresML, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: PostgresML
provider_slug: postgresml
slug: postgresml-domain-security
source_filename: postgresml-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: postgresml.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 10:13:20 2026 GMT\n  hsts: false\ndomains:\n- domain: postgresml.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/postgresml/refs/heads/main/security/postgresml-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Ai Ml
- Machine Learning
- Vector Search
- Embeddings
- PostgreSQL
- RAG
- LLM
- Database
---
