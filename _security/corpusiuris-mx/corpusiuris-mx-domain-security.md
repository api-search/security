---
api_specs:
- filename: corpusiuris-mx-agent-api-openapi.yml
  format: yaml
  label: Corpus Iuris Agent API
  slug: corpusiuris-mx-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corpusiuris-mx/openapi/corpusiuris-mx-agent-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: corpusiuris.mx
  spf: true
hosts:
- cert_expires: Feb  1 06:02:25 2027 GMT
  host: corpusiuris.mx
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Corpus Iuris Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Corpus Iuris, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Corpus Iuris
provider_slug: corpusiuris-mx
slug: corpusiuris-mx-domain-security
source_filename: corpusiuris-mx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: corpusiuris.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 06:02:25 2027 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: corpusiuris.mx\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/corpusiuris-mx/security/corpusiuris-mx-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Legal
- Legal Research
- Artificial Intelligence
- Mexico
- Jurisprudence
- MCP
- Search
---
