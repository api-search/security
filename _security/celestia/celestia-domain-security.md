---
api_specs:
- filename: celestia-blob-api-openapi.yml
  format: yaml
  label: Celestia Node Blob API
  slug: celestia-blob-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/celestia/openapi/celestia-blob-api-openapi.yml
- filename: celestia-contact-api-openapi.yml
  format: yaml
  label: Celestia Contact API
  slug: celestia-contact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/celestia/openapi/celestia-contact-api-openapi.yml
- filename: celestia-health-api-openapi.yml
  format: yaml
  label: Celestia Health API
  slug: celestia-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/celestia/openapi/celestia-health-api-openapi.yml
- filename: celestia-subscribe-api-openapi.yml
  format: yaml
  label: Celestia Subscribe API
  slug: celestia-subscribe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/celestia/openapi/celestia-subscribe-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: true
  domain: celestia.org
  spf: true
hosts:
- cert_expires: Nov 27 05:56:29 2026 GMT
  host: www.celestia.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 05:56:29 2026 GMT
  host: celestia.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: node-rpc-docs.celestia.org
  https: false
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Celestia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Celestia, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present.'
provider_name: Celestia
provider_slug: celestia
slug: celestia-domain-security
source_filename: celestia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.celestia.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 05:56:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: celestia.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 05:56:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: node-rpc-docs.celestia.org\n  https: false\ndomains:\n- domain: celestia.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n"
source_yaml_url: https://artifacts.apis.io/celestia/security/celestia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- Data Availability
- Web3
- Infrastructure
- Open Source
- JSON-RPC
- Modular Blockchain
- Rollup
- Cryptography
- Developer Tools
---
