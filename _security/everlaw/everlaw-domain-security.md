---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Everlaw REST API
  slug: everlaw-rest-api
  spec_type: OpenAPI
  url: https://api.everlaw.com/docs/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: everlaw.com
  spf: true
hosts:
- cert_expires: Aug 23 03:35:48 2026 GMT
  host: www.everlaw.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: api.everlaw.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Everlaw Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Everlaw, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Everlaw
provider_slug: everlaw
slug: everlaw-domain-security
source_filename: everlaw-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.everlaw.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 03:35:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.everlaw.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: everlaw.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/everlaw/refs/heads/main/security/everlaw-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- eDiscovery
- Litigation
- Legal Technology
- Document Review
- Predictive Coding
- AI
- Legal
---
