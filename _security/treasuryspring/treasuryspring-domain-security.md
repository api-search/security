---
api_specs:
- filename: treasuryspring-openapi-original.json
  format: json
  label: TreasurySpring Public API
  slug: treasuryspring-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/treasuryspring/refs/heads/main/openapi/treasuryspring-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: treasuryspring.com
  spf: true
hosts:
- cert_expires: Sep 17 19:02:52 2026 GMT
  host: www.treasuryspring.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: api.treasuryspring.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: api.sandbox.treasuryspring.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Treasuryspring Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TreasurySpring, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TreasurySpring
provider_slug: treasuryspring
slug: treasuryspring-domain-security
source_filename: treasuryspring-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.treasuryspring.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 19:02:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.treasuryspring.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: null\n- host: api.sandbox.treasuryspring.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: treasuryspring.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/treasuryspring/refs/heads/main/security/treasuryspring-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Cash Management
- Treasury
- Investments
- Financial Services
- Fixed Term Funds
- Payments
- MCP
---
