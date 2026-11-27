---
api_specs:
- filename: jamp-io-openapi-generated.yml
  format: yaml
  label: JAMP API
  slug: jamp-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jamp-io/openapi/_ae-authored/jamp-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: jamp.io
  spf: true
hosts:
- cert_expires: Jan  7 14:20:50 2027 GMT
  host: jamp.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: JAMP Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JAMP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: JAMP
provider_slug: jamp-io
slug: jamp-io-domain-security
source_filename: jamp-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jamp.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 14:20:50 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: jamp.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/jamp-io/security/jamp-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Analytics
- Monitoring
- Privacy
- Artificial Intelligence
- Web
---
