---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: stashapp.cc
  spf: true
hosts:
- cert_expires: Dec 17 12:15:21 2026 GMT
  host: stashapp.cc
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Stashapp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stash, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Stash
provider_slug: stashapp
slug: stashapp-domain-security
source_filename: stashapp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stashapp.cc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 12:15:21 2026 GMT\n  hsts: false\ndomains:\n- domain: stashapp.cc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/stashapp/security/stashapp-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Media
- Open-source
- Adult
- Organizer
---
