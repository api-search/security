---
api_specs:
- filename: polycode-co-uk-marginalia-openapi.json
  format: json
  label: marginalia public API
  slug: marginalia-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polycode-co-uk/refs/heads/main/openapi/polycode-co-uk-marginalia-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: polycode.co.uk
  spf: false
hosts:
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: marginalia.polycode.co.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Polycode Co Uk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Polycode, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Polycode
provider_slug: polycode-co-uk
slug: polycode-co-uk-domain-security
source_filename: polycode-co-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: marginalia.polycode.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: polycode.co.uk\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polycode-co-uk/refs/heads/main/security/polycode-co-uk-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Chat
- Memory
- Agents
- A2A
- Knowledge Graph
- Research
- Artificial Intelligence
- Open Source
- Consulting
- United Kingdom
---
