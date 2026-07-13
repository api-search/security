---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: json-schema.org
  spf: true
hosts:
- cert_expires: Sep 15 14:40:36 2026 GMT
  host: json-schema.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Json Schema Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JSON Schema, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: JSON Schema
provider_slug: json-schema
slug: json-schema-domain-security
source_filename: json-schema-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: json-schema.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 14:40:36 2026 GMT\n  hsts: false\ndomains:\n- domain: json-schema.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/json-schema/refs/heads/main/security/json-schema-domain-security.yml
summary_line: TLSv1.3
tags:
- API Design
- Specification Language
- JSON
- Validation
- Schema
---
