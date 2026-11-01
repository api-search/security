---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: pixelvault.dev
  spf: true
hosts:
- cert_expires: Dec  7 10:03:29 2026 GMT
  host: pixelvault.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pixelvault Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for pixelvault-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: pixelvault-dev
provider_slug: pixelvault-dev
slug: pixelvault-dev-domain-security
source_filename: pixelvault-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pixelvault.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 10:03:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pixelvault.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/pixelvault-dev/security/pixelvault-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Image Hosting
- CDN
- API
- AI Agents
- Developer Tools
---
