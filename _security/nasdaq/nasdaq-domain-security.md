---
api_specs:
- filename: nasdaq-asyncapi.yml
  format: yaml
  label: Nasdaq Cloud Data Service (NCDS) — Kafka Streams
  slug: nasdaq-cloud-data-service-ncds-kafka-streams
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasdaq/refs/heads/main/asyncapi/nasdaq-asyncapi.yml
- filename: nasdaq-ncds-rest-postman-collection.json
  format: json
  label: Nasdaq Cloud Data Service (NCDS) REST API
  slug: nasdaq-cloud-data-service-ncds-rest-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/nasdaq/refs/heads/main/postman/nasdaq-ncds-rest-postman-collection.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nasdaq.com
  spf: true
hosts:
- cert_expires: Feb 12 23:59:59 2027 GMT
  host: www.nasdaq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: streams.ncds.nasdaq.com
  https: false
- cert_expires: Nov  3 08:09:19 2026 GMT
  host: data.nasdaq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Nasdaq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nasdaq, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nasdaq
provider_slug: nasdaq
slug: nasdaq-domain-security
source_filename: nasdaq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nasdaq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 23:59:59 2027 GMT\n  hsts: false\n- host: streams.ncds.nasdaq.com\n  https: false\n- host: data.nasdaq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 08:09:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nasdaq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nasdaq/refs/heads/main/security/nasdaq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Marketplace
- Financial Data
- Fortune 1000
- Kafka
- Market Data
- Stock Exchange
- Streaming
---
