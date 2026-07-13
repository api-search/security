---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openapis.org
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: asyncapi.com
  spf: false
hosts:
- cert_expires: Sep  6 18:54:28 2026 GMT
  host: www.openapis.org
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 05:12:18 2026 GMT
  host: spec.openapis.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 03:28:50 2026 GMT
  host: www.asyncapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Test Specifications Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Test Specifications, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Test Specifications
provider_slug: test-specifications
slug: test-specifications-domain-security
source_filename: test-specifications-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.openapis.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 18:54:28 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: spec.openapis.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 05:12:18 2026 GMT\n  hsts: false\n- host: www.asyncapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 03:28:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: openapis.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: asyncapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/test-specifications/refs/heads/main/security/test-specifications-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Acceptance Testing
- Contract Testing
- Documentation
- OpenAPI
- Quality Assurance
- Testing
---
