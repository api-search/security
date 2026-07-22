---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: presence.io
  spf: true
hosts:
- cert_expires: Oct 13 13:02:40 2026 GMT
  host: presence.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Presence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Presence, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Open Presence
provider_slug: open-presence
slug: open-presence-domain-security
source_filename: open-presence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: presence.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 13:02:40 2026 GMT\n  hsts: null\ndomains:\n- domain: presence.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-presence/refs/heads/main/security/open-presence-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
