---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hydrant.dev
  spf: true
hosts:
- cert_expires: Dec 13 03:24:18 2026 GMT
  host: hydrant.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hydrant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hydrant, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hydrant
provider_slug: hydrant-dev
slug: hydrant-dev-domain-security
source_filename: hydrant-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hydrant.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 03:24:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hydrant.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/hydrant-dev/security/hydrant-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Collaboration
- Project Management
- Artificial Intelligence
- Issue Tracking
- Software-as-a-Service
---
