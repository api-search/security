---
api_specs:
- filename: futureagi-api-openapi.json
  format: json
  label: Future AGI API API
  slug: future-agi-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/futureagi/openapi/_original/futureagi-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: futureagi.com
  spf: true
hosts:
- cert_expires: May  3 23:59:59 2027 GMT
  host: futureagi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Futureagi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Future AGI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Future AGI
provider_slug: futureagi
slug: futureagi-domain-security
source_filename: futureagi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: futureagi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May  3 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: futureagi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/futureagi/security/futureagi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Platform
- Agents
- Simulation
- Monitoring
---
