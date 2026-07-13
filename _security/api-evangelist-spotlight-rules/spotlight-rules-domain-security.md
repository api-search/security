---
api_specs:
- filename: spotlight-rules-openapi.yml
  format: yaml
  label: Spotlight Rules Feed
  slug: spotlight-rules
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-evangelist-spotlight-rules/refs/heads/main/openapi/spotlight-rules-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: spotlight-rules.com
  spf: false
hosts:
- cert_expires: Aug 12 22:17:27 2026 GMT
  host: spotlight-rules.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spotlight Rules Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spotlight Rules, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Spotlight Rules
provider_slug: api-evangelist-spotlight-rules
slug: spotlight-rules-domain-security
source_filename: spotlight-rules-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spotlight-rules.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 22:17:27 2026 GMT\n  hsts: null\ndomains:\n- domain: spotlight-rules.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-evangelist-spotlight-rules/refs/heads/main/security/spotlight-rules-domain-security.yml
summary_line: TLSv1.3
tags:
- Rules
- Spotlight
- Governance
---
