---
api_specs:
- filename: seon-docs-openapi.yml
  format: yaml
  label: SEON Fraud API
  slug: fraud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seon-docs/refs/heads/main/openapi/seon-docs-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: seon.io
  spf: true
hosts:
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: docs.seon.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 18 15:25:59 2026 GMT
  host: seon.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: api.seon.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Seon Docs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SEON, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: SEON
provider_slug: seon-docs
slug: seon-docs-domain-security
source_filename: seon-docs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.seon.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: seon.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 15:25:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.seon.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: seon.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seon-docs/refs/heads/main/security/seon-docs-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- AML Compliance
- Fraud Prevention
- Identity Verification
- Risk Scoring
---
