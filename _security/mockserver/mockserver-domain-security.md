---
api_specs:
- filename: mockserver-openapi-original.yml
  format: yaml
  label: MockServer
  slug: mockserver
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mockserver/refs/heads/main/openapi/mockserver-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: mock-server.com
  spf: false
hosts:
- cert_expires: Sep 16 23:59:59 2026 GMT
  host: www.mock-server.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mockserver Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MockServer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=quarantine).'
provider_name: MockServer
provider_slug: mockserver
slug: mockserver-domain-security
source_filename: mockserver-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mock-server.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mock-server.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issue \"amazon.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mockserver/refs/heads/main/security/mockserver-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Mocking
- Mock Server
- Testing
- Service Virtualization
- HTTP
- REST API
- Platform
---
