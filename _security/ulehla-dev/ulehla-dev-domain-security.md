---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ulehla.dev
  spf: true
hosts:
- cert_expires: Dec 12 08:44:06 2026 GMT
  host: ulehla.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ulehla Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ulehla-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ulehla-dev
provider_slug: ulehla-dev
slug: ulehla-dev-domain-security
source_filename: ulehla-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ulehla.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 08:44:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ulehla.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/ulehla-dev/security/ulehla-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fullstack
- AI Engineer
- Developer
- Personal Site
- Open Source
---
