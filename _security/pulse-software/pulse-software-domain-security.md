---
api_specs:
- filename: pulse-software-openapi.yml
  format: yaml
  label: Pulse Software
  slug: pulse-software
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pulse-software/refs/heads/main/openapi/pulse-software-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pulsesoftware.com
  spf: true
hosts:
- cert_expires: Sep  2 07:34:03 2026 GMT
  host: apidoc.pulsesoftware.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: '*.pulsesoftware.com'
  https: false
kind: domain-security
layout: security
method: probed
name: Pulse Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pulse Software, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pulse Software
provider_slug: pulse-software
slug: pulse-software-domain-security
source_filename: pulse-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apidoc.pulsesoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 07:34:03 2026 GMT\n  hsts: false\n- host: '*.pulsesoftware.com'\n  https: false\ndomains:\n- domain: pulsesoftware.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pulse-software/refs/heads/main/security/pulse-software-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Pulse
- Automation
- Developer
---
