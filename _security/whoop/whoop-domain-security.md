---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: WHOOP API
  slug: whoop-api
  spec_type: OpenAPI
  url: https://developer.whoop.com/api/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: whoop.com
  spf: true
hosts:
- cert_expires: Oct  4 14:39:54 2026 GMT
  host: www.whoop.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: developer.whoop.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 00:33:36 2026 GMT
  host: api.prod.whoop.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Whoop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WHOOP, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: WHOOP
provider_slug: whoop
slug: whoop-domain-security
source_filename: whoop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.whoop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 14:39:54 2026 GMT\n  hsts: false\n- host: developer.whoop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: false\n- host: api.prod.whoop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 00:33:36 2026 GMT\n  hsts: null\ndomains:\n- domain: whoop.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whoop/refs/heads/main/security/whoop-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fitness
- Wearables
- Health
- Recovery
- Sleep
- Workout
- Strain
- Heart Rate
- Performance
---
