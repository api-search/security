---
api_specs:
- filename: opsmill-infrahub-openapi-original.json
  format: json
  label: Infrahub REST API
  slug: infrahub-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsmill/refs/heads/main/openapi/opsmill-infrahub-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: opsmill.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: infrahub.app
  spf: false
hosts:
- cert_expires: Aug 30 18:11:12 2026 GMT
  host: opsmill.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 15:17:56 2026 GMT
  host: docs.infrahub.app
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 02:15:34 2026 GMT
  host: sandbox.infrahub.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opsmill Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpsMill, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OpsMill
provider_slug: opsmill
slug: opsmill-domain-security
source_filename: opsmill-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opsmill.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 18:11:12 2026 GMT\n  hsts: false\n- host: docs.infrahub.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 15:17:56 2026 GMT\n  hsts: false\n- host: sandbox.infrahub.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 02:15:34 2026 GMT\n  hsts: null\ndomains:\n- domain: opsmill.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: infrahub.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opsmill/refs/heads/main/security/opsmill-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Infrastructure Saas
- Network Automation
- Source Of Truth
- Data Management
- GraphQL
- DevOps
- Configuration Management
- AIOps
- Open Source
---
