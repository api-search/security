---
api_specs:
- filename: nma_swagger.json
  format: json
  label: Vertica Node Management Agent API
  slug: node-management-agent-api
  spec_type: OpenAPI
  url: https://<node-host>:5554/api-docs/nma_swagger.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vertica.com
  spf: true
hosts:
- cert_expires: Sep  3 21:30:49 2026 GMT
  host: www.vertica.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  9 23:59:59 2027 GMT
  host: docs.vertica.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vertica Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vertica, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vertica
provider_slug: vertica
slug: vertica-domain-security
source_filename: vertica-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vertica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 21:30:49 2026 GMT\n  hsts: null\n- host: docs.vertica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  9 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: vertica.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vertica/refs/heads/main/security/vertica-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Database
- Analytics Database
- Data Warehouse
- Data Lakehouse
- Columnar Database
- MPP
- In-Database Machine Learning
- SQL
---
