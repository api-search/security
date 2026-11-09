---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: devplane.dev
  spf: false
hosts:
- cert_expires: Dec  5 20:00:29 2026 GMT
  host: devplane.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Devplane Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DevPlane, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: DevPlane
provider_slug: devplane-dev
slug: devplane-dev-domain-security
source_filename: devplane-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: devplane.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 20:00:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: devplane.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/devplane-dev/security/devplane-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Development
- Platform
- Developer Tools
---
