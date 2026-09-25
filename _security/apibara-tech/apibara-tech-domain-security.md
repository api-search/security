---
api_specs:
- filename: apibara-tech-openapi.json
  format: json
  label: Vehicle Auction Data API
  slug: vehicle-auction-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apibara-tech/refs/heads/main/openapi/apibara-tech-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: apibara.tech
  spf: true
hosts:
- cert_expires: Nov 22 10:00:33 2026 GMT
  host: apibara.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Apibara Tech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apibara.tech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Apibara.tech
provider_slug: apibara-tech
slug: apibara-tech-domain-security
source_filename: apibara-tech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apibara.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 10:00:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apibara.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apibara-tech/refs/heads/main/security/apibara-tech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automotive
- vehicle-auction-data
- Copart
- IAAI
- vin-history
- Marketplace
- REST API
- Vehicle Auctions
- Salvage Auctions
- VIN Data
- Used-Car Marketplace Data
- Data Infrastructure
- Data as a Service
- REST
- JSON:API
- MCP
- Agent-Native
---
