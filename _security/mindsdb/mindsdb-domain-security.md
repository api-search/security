---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mindshub.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mindsdb.com
  spf: true
hosts:
- cert_expires: Oct  9 02:14:51 2026 GMT
  host: mindshub.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 00:30:57 2026 GMT
  host: docs.mindsdb.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 23:59:59 2026 GMT
  host: cloud.mindsdb.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mindsdb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MindsDB, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MindsDB
provider_slug: mindsdb
slug: mindsdb-domain-security
source_filename: mindsdb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mindshub.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 02:14:51 2026 GMT\n  hsts: false\n- host: docs.mindsdb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 00:30:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: cloud.mindsdb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: mindshub.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: mindsdb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mindsdb/refs/heads/main/security/mindsdb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- AI Agents
- Data
- Database
- SQL
- Knowledge Base
- MCP
- Open Source
---
