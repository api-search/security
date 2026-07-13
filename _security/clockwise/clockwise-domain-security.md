---
api_specs:
- filename: openapi.yml
  format: yaml
  label: Clockwise REST API
  slug: clockwise-rest-api
  spec_type: OpenAPI
  url: https://api.getclockwise.com/openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: getclockwise.com
  spf: true
hosts:
- cert_expires: Aug 29 16:02:11 2026 GMT
  host: www.getclockwise.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.getclockwise.com
  https: false
kind: domain-security
layout: security
method: probed
name: Clockwise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clockwise, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Clockwise
provider_slug: clockwise
slug: clockwise-domain-security
source_filename: clockwise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getclockwise.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 16:02:11 2026 GMT\n  hsts: false\n- host: api.getclockwise.com\n  https: false\ndomains:\n- domain: getclockwise.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clockwise/refs/heads/main/security/clockwise-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Calendar
- AI
- Scheduling
- Focus Time
- Productivity
- Team Coordination
- Meeting Optimization
---
