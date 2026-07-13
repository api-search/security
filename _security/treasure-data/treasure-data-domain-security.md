---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Treasure Data TD API
  slug: treasure-data-td-api
  spec_type: OpenAPI
  url: https://api-docs.treasuredata.com/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: treasure.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: treasuredata.com
  spf: true
hosts:
- cert_expires: Aug 27 22:09:16 2026 GMT
  host: www.treasure.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 02:37:07 2026 GMT
  host: docs.treasure.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 23:59:59 2026 GMT
  host: api.treasuredata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Treasure Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Treasure Data, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Treasure Data
provider_slug: treasure-data
slug: treasure-data-domain-security
source_filename: treasure-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.treasure.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 22:09:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.treasure.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 02:37:07 2026 GMT\n  hsts: false\n- host: api.treasuredata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: treasure.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: treasuredata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/treasure-data/refs/heads/main/security/treasure-data-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Customer Data Platform
- CDP
- Big Data
- Data Warehouse
- Hive
- Presto
- Enterprise
- AI
- Marketing
- Analytics
---
