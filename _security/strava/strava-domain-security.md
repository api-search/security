---
api_specs:
- filename: strava-openapi.yml
  format: yaml
  label: Strava API
  slug: strava
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/strava/refs/heads/main/openapi/strava-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: strava.com
  spf: true
hosts:
- cert_expires: Sep 23 13:15:48 2026 GMT
  host: www.strava.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 13:15:48 2026 GMT
  host: developers.strava.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Strava Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Strava, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Strava
provider_slug: strava
slug: strava-domain-security
source_filename: strava-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.strava.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 13:15:48 2026 GMT\n  hsts: false\n- host: developers.strava.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 23 13:15:48 2026 GMT\n  hsts: false\ndomains:\n- domain: strava.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/strava/refs/heads/main/security/strava-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cycling
- Fitness
- Fitness Tracking
- Running
- Sports
---
