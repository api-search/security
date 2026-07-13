---
api_specs:
- filename: swagger.json
  format: json
  label: Orbit REST API
  slug: orbit-rest-api
  spec_type: OpenAPI
  url: https://app.orbit.love/api-docs/v1/swagger.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: orbit.love
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: archive.org
  spf: true
hosts:
- cert_expires: Aug 27 08:45:47 2026 GMT
  host: orbit.love
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 08:45:47 2026 GMT
  host: app.orbit.love
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  9 22:02:42 2027 GMT
  host: web.archive.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Orbit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orbit, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Orbit
provider_slug: orbit
slug: orbit-domain-security
source_filename: orbit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: orbit.love\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 08:45:47 2026 GMT\n  hsts: null\n- host: app.orbit.love\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 08:45:47 2026 GMT\n  hsts: null\n- host: web.archive.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 22:02:42 2027 GMT\n  hsts: false\ndomains:\n- domain: orbit.love\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: archive.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orbit/refs/heads/main/security/orbit-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Developer Relations
- Community Intelligence
- DevRel
- Community Management
- Member Tracking
- Community Analytics
- Open Source
- Developer Engagement
---
