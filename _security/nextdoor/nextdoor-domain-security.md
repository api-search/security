---
api_specs:
- filename: nextdoor-openapi.yml
  format: yaml
  label: Nextdoor
  slug: nextdoor
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdoor/refs/heads/main/openapi/nextdoor-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nextdoor.com
  spf: true
hosts:
- cert_expires: Sep 13 18:58:38 2026 GMT
  host: developer.nextdoor.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nextdoor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nextdoor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nextdoor
provider_slug: nextdoor
slug: nextdoor-domain-security
source_filename: nextdoor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.nextdoor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 18:58:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nextdoor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nextdoor/refs/heads/main/security/nextdoor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Social
- Local
- Advertising
- Community
- Sharing
---
