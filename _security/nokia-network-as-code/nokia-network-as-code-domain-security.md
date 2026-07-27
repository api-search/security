---
api_specs:
- filename: nokia-network-as-code-platform-openapi.json
  format: json
  label: Nokia Network as Code Platform API
  slug: network-as-code-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nokia-network-as-code/refs/heads/main/openapi/nokia-network-as-code-platform-openapi.json
- filename: nokia-network-as-code-camara-openapi.yml
  format: yaml
  label: Nokia Network as Code CAMARA API
  slug: camara-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nokia-network-as-code/refs/heads/main/openapi/nokia-network-as-code-camara-openapi.yml
- filename: nokia-network-as-code-platform-openapi.json
  format: json
  label: Network as Code Digital Identity and Anti-Fraud APIs
  slug: digital-identity-and-anti-fraud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nokia-network-as-code/refs/heads/main/openapi/nokia-network-as-code-platform-openapi.json
- filename: nokia-network-as-code-platform-openapi.json
  format: json
  label: Network as Code Device Intelligence APIs
  slug: device-intelligence
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nokia-network-as-code/refs/heads/main/openapi/nokia-network-as-code-platform-openapi.json
- filename: nokia-network-as-code-platform-openapi.json
  format: json
  label: Network as Code Programmable Connectivity APIs
  slug: programmable-connectivity
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nokia-network-as-code/refs/heads/main/openapi/nokia-network-as-code-platform-openapi.json
- filename: nokia-network-as-code-platform-openapi.json
  format: json
  label: Network as Code Network Intelligence APIs
  slug: network-intelligence
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nokia-network-as-code/refs/heads/main/openapi/nokia-network-as-code-platform-openapi.json
- filename: nokia-network-as-code-platform-openapi.json
  format: json
  label: Network as Code Authorization Server
  slug: authorization-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nokia-network-as-code/refs/heads/main/openapi/nokia-network-as-code-platform-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nokia.io
  spf: false
- caa: []
  dmarc: false
  dnssec: true
  domain: rapidapi.com
  spf: true
hosts:
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: networkascode.nokia.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 10:46:02 2026 GMT
  host: network-as-code.p-eu.rapidapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nokia Network As Code Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nokia Network as Code, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Nokia Network as Code
provider_slug: nokia-network-as-code
slug: nokia-network-as-code-domain-security
source_filename: nokia-network-as-code-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: networkascode.nokia.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: network-as-code.p-eu.rapidapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 10:46:02 2026 GMT\n  hsts: null\ndomains:\n- domain: nokia.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n- domain: rapidapi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nokia-network-as-code/refs/heads/main/security/nokia-network-as-code-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Telecommunications
- Finland
- Network APIs
- CAMARA
- Open Gateway
- Network API Exposure
- Network API Aggregator
- 5G
- Identity Verification
- SIM Swap
- Number Verification
- Device Location
- Quality on Demand
- Network Slicing
- Anti-Fraud
- KYC
- IoT
- eSIM
- Roaming
- Network Exposure
---
