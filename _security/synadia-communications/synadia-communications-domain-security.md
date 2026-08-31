---
api_specs:
- filename: synadia-communications-control-plane-openapi.yaml
  format: yaml
  label: Synadia Control Plane / Synadia Cloud API
  slug: synadia-communications-control-plane
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synadia-communications/refs/heads/main/openapi/synadia-communications-control-plane-openapi.yaml
- filename: synadia-communications-http-gateway-openapi.json
  format: json
  label: Synadia Cloud NATS HTTP Gateway
  slug: synadia-communications-http-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synadia-communications/refs/heads/main/openapi/synadia-communications-http-gateway-openapi.json
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: synadia.com
  spf: true
hosts:
- cert_expires: Nov 21 07:59:01 2026 GMT
  host: www.synadia.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 14 23:59:59 2027 GMT
  host: cloud.synadia.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 00:45:07 2026 GMT
  host: docs.synadia.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Synadia Communications Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Synadia Communications, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Synadia Communications
provider_slug: synadia-communications
slug: synadia-communications-domain-security
source_filename: synadia-communications-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.synadia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 07:59:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: cloud.synadia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 23:59:59 2027 GMT\n  hsts: null\n- host: docs.synadia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 00:45:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: synadia.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synadia-communications/refs/heads/main/security/synadia-communications-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Messaging
- Event Streaming
- NATS
- Distributed Systems
- Edge Computing
- Publish Subscribe
- Key Value Store
- Object Storage
- Infrastructure
- Agentic AI
- Open Source
---
