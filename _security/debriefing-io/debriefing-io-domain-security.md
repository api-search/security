---
api_specs:
- filename: debriefing-io-openapi.json
  format: json
  label: Debriefing Read API
  slug: debriefing-read-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debriefing-io/openapi/debriefing-io-openapi.json
- filename: debriefing-io-battlecards-api-openapi.yml
  format: yaml
  label: Debriefing Battlecards API
  slug: debriefing-io-battlecards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debriefing-io/openapi/debriefing-io-battlecards-api-openapi.yml
- filename: debriefing-io-competitors-api-openapi.yml
  format: yaml
  label: Debriefing Competitors API
  slug: debriefing-io-competitors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debriefing-io/openapi/debriefing-io-competitors-api-openapi.yml
- filename: debriefing-io-digests-api-openapi.yml
  format: yaml
  label: Debriefing Digests API
  slug: debriefing-io-digests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debriefing-io/openapi/debriefing-io-digests-api-openapi.yml
- filename: debriefing-io-signals-api-openapi.yml
  format: yaml
  label: Debriefing Signals API
  slug: debriefing-io-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/debriefing-io/openapi/debriefing-io-signals-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: debriefing.io
  spf: true
hosts:
- cert_expires: Dec 12 00:01:18 2026 GMT
  host: debriefing.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Debriefing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Debriefing, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Debriefing
provider_slug: debriefing-io
slug: debriefing-io-domain-security
source_filename: debriefing-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: debriefing.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 00:01:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: debriefing.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/debriefing-io/security/debriefing-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Competitive Intelligence
- Software-as-a-Service
- B2B
- Monitoring
- Small Business
---
