---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: restfulapi.net
  spf: true
hosts:
- cert_expires: Sep  3 23:14:49 2026 GMT
  host: restfulapi.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rest Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for REST API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: REST API
provider_slug: rest-api
slug: rest-api-domain-security
source_filename: rest-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: restfulapi.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 23:14:49 2026 GMT\n  hsts: false\ndomains:\n- domain: restfulapi.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rest-api/refs/heads/main/security/rest-api-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Architecture
- HTTP
- Web Services
- REST
- API Design
---
