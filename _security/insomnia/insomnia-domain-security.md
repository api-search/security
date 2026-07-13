---
api_specs:
- filename: insomnia-mock-server-openapi.yml
  format: yaml
  label: Insomnia Mock Server API
  slug: mock-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insomnia/refs/heads/main/openapi/insomnia-mock-server-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: konghq.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: insomnia.rest
  spf: true
hosts:
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: konghq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 09:01:57 2026 GMT
  host: insomnia.rest
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 01:06:23 2026 GMT
  host: docs.insomnia.rest
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Insomnia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Insomnia, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Insomnia
provider_slug: insomnia
slug: insomnia-domain-security
source_filename: insomnia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: konghq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: false\n- host: insomnia.rest\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 09:01:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.insomnia.rest\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 01:06:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: konghq.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: insomnia.rest\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/insomnia/refs/heads/main/security/insomnia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- API Design
- CLI
- Clients
- Mocking
- Platform
- Testing
---
