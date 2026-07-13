---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: uuidtools.com
  spf: false
hosts:
- cert_expires: Aug 21 00:11:12 2026 GMT
  host: www.uuidtools.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uuid Generator Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UUID Generator, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: UUID Generator
provider_slug: uuid-generator
slug: uuid-generator-domain-security
source_filename: uuid-generator-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uuidtools.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 00:11:12 2026 GMT\n  hsts: false\ndomains:\n- domain: uuidtools.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uuid-generator/refs/heads/main/security/uuid-generator-domain-security.yml
summary_line: TLSv1.3
tags:
- Test Data
- Public APIs
---
