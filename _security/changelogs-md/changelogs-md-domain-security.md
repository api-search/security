---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: changelogs.md
  spf: true
hosts:
- cert_expires: Oct  9 14:15:33 2026 GMT
  host: changelogs.md
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Changelogs Md Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Changelogs.md, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Changelogs.md
provider_slug: changelogs-md
slug: changelogs-md-domain-security
source_filename: changelogs-md-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: changelogs.md\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  9 14:15:33 2026 GMT\n  hsts: false\ndomains:\n- domain: changelogs.md\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/changelogs-md/refs/heads/main/security/changelogs-md-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Development
- Public APIs
---
