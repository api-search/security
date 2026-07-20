---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dremio.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: dremio.cloud
  spf: false
hosts:
- cert_expires: Sep 15 19:01:38 2026 GMT
  host: docs.dremio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: api.dremio.cloud
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dremio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dremio, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dremio
provider_slug: dremio
slug: dremio-domain-security
source_filename: dremio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.dremio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 19:01:38 2026 GMT\n  hsts: false\n- host: api.dremio.cloud\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: dremio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: dremio.cloud\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dremio/refs/heads/main/security/dremio-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Data Lakehouse
- Analytics
- SQL Query Engine
- Apache Iceberg
- Apache Arrow
- Data Catalog
- Semantic Layer
- AI Agents
- MCP
---
