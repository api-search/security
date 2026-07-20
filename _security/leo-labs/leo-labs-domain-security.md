---
api_specs:
- filename: leo-labs-platform-openapi.yml
  format: yaml
  label: LeoLabs Platform API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leo-labs/refs/heads/main/openapi/leo-labs-platform-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: leolabs.space
  spf: true
hosts:
- cert_expires: Aug 27 14:23:41 2026 GMT
  host: www.leolabs.space
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: api.leolabs.space
  hsts: true
  hsts_max_age: 315360000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Leo Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LeoLabs, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: LeoLabs
provider_slug: leo-labs
slug: leo-labs-domain-security
source_filename: leo-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.leolabs.space\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 14:23:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.leolabs.space\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 315360000\ndomains:\n- domain: leolabs.space\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leo-labs/refs/heads/main/security/leo-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Space
- Satellites
- Space Situational Awareness
- Space Traffic Management
- Orbital Data
- Radar
- Aerospace
- Defense
- Geospatial
---
