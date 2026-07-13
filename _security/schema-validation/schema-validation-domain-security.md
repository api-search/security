---
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: false
  dnssec: false
  domain: json-schema.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: js.org
  spf: true
hosts:
- cert_expires: Sep 15 14:40:36 2026 GMT
  host: json-schema.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 14:27:59 2026 GMT
  host: ajv.js.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 18:19:40 2026 GMT
  host: json-schema.hyperjump.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Schema Validation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Schema Validation, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Schema Validation
provider_slug: schema-validation
slug: schema-validation-domain-security
source_filename: schema-validation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: json-schema.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 14:40:36 2026 GMT\n  hsts: false\n- host: ajv.js.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 14:27:59 2026 GMT\n  hsts: false\n- host: json-schema.hyperjump.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 18:19:40 2026 GMT\n  hsts: false\ndomains:\n- domain: json-schema.org\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: false\n- domain: js.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/schema-validation/refs/heads/main/security/schema-validation-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- API Governance
- Contract Testing
- JSON Schema
- OpenAPI
- Schema Validation
---
