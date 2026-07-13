---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openapis.org
  spf: true
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
kind: domain-security
layout: security
method: probed
name: Openapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenAPI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OpenAPI
provider_slug: openapi
slug: openapi-domain-security
source_filename: openapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.openapis.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 18:54:28 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: spec.openapis.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 05:12:18 2026 GMT\n  hsts: false\ndomains:\n- domain: openapis.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openapi/refs/heads/main/security/openapi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Documentation
- REST
- Specification
---
