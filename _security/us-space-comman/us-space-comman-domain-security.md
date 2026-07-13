---
api_specs:
- filename: us-space-command-space-track-openapi.yml
  format: yaml
  label: Space-Track.org REST API
  slug: space-track-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-space-comman/refs/heads/main/openapi/us-space-command-space-track-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: space-track.org
  spf: true
hosts:
- cert_expires: Sep  1 06:41:10 2026 GMT
  host: www.space-track.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Us Space Comman Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for US Space Command, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: US Space Command
provider_slug: us-space-comman
slug: us-space-comman-domain-security
source_filename: us-space-comman-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.space-track.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 06:41:10 2026 GMT\n  hsts: false\ndomains:\n- domain: space-track.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-space-comman/refs/heads/main/security/us-space-comman-domain-security.yml
summary_line: TLSv1.3
tags:
- Federal Government
- Space
- Space Situational Awareness
- Satellite Tracking
- Open Data
---
