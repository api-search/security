---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: spear.dev
  spf: true
hosts:
- cert_expires: Oct 12 15:16:16 2026 GMT
  host: spear.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spear Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spear, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Spear
provider_slug: spear
slug: spear-domain-security
source_filename: spear-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spear.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 15:16:16 2026 GMT\n  hsts: false\ndomains:\n- domain: spear.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spear/refs/heads/main/security/spear-domain-security.yml
summary_line: TLSv1.3
tags:
- API Development
- Collaboration
- Developer Tools
- Platform
---
