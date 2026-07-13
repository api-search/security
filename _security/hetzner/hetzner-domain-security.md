---
api_specs:
- filename: hetzner-openapi.yml
  format: yaml
  label: Hetzner Cloud API
  slug: hetzner-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hetzner/refs/heads/main/openapi/hetzner-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hetzner.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: hetzner.cloud
  spf: false
hosts:
- cert_expires: Aug 13 23:59:59 2026 GMT
  host: www.hetzner.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 10:50:03 2026 GMT
  host: docs.hetzner.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 08:34:28 2026 GMT
  host: api.hetzner.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hetzner Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hetzner, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hetzner
provider_slug: hetzner
slug: hetzner-domain-security
source_filename: hetzner-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hetzner.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.hetzner.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 10:50:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.hetzner.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 08:34:28 2026 GMT\n  hsts: null\ndomains:\n- domain: hetzner.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: hetzner.cloud\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hetzner/refs/heads/main/security/hetzner-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Hosting
- DNS
- Infrastructure
- Servers
---
