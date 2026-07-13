---
api_specs:
- filename: stardog-openapi.json
  format: json
  label: Stardog HTTP API
  slug: http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stardog/refs/heads/main/openapi/stardog-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: stardog.com
  spf: true
hosts:
- cert_expires: Sep  7 14:00:44 2026 GMT
  host: www.stardog.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: cloud.stardog.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Stardog Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stardog, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Stardog
provider_slug: stardog
slug: stardog-domain-security
source_filename: stardog-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stardog.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 14:00:44 2026 GMT\n  hsts: false\n- host: cloud.stardog.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: stardog.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stardog/refs/heads/main/security/stardog-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Knowledge Graph
- Graph Database
- Semantic Web
- SPARQL
- Data Virtualization
- Enterprise Data
---
