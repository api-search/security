---
api_specs:
- filename: vast-space-openapi.yml
  format: yaml
  label: Vast Haven-1 Station
  slug: haven-1-station
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vast-space/refs/heads/main/openapi/vast-space-openapi.yml
- filename: vast-space-openapi.yml
  format: yaml
  label: Vast Haven-2 Station
  slug: haven-2-station
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vast-space/refs/heads/main/openapi/vast-space-openapi.yml
- filename: vast-space-openapi.yml
  format: yaml
  label: Vast Haven-1 Lab
  slug: haven-1-lab
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vast-space/refs/heads/main/openapi/vast-space-openapi.yml
- filename: vast-space-openapi.yml
  format: yaml
  label: Vast Payload & Research Opportunities
  slug: payload-research-opportunities
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vast-space/refs/heads/main/openapi/vast-space-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: vastspace.com
  spf: true
hosts:
- cert_expires: Sep 30 21:15:03 2026 GMT
  host: www.vastspace.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vast Space Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vast, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Vast
provider_slug: vast-space
slug: vast-space-domain-security
source_filename: vast-space-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vastspace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 21:15:03 2026 GMT\n  hsts: false\ndomains:\n- domain: vastspace.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vast-space/refs/heads/main/security/vast-space-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Space
- Aerospace
- Space Station
- Human Spaceflight
- Microgravity
- Research
- Informational
---
