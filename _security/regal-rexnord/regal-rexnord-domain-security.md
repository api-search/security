---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: regalrexnord.com
  spf: true
hosts:
- cert_expires: Sep 25 22:25:57 2026 GMT
  host: www.regalrexnord.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: developer.regalrexnord.com
  https: false
- host: api.regalrexnord.com
  https: false
kind: domain-security
layout: security
method: probed
name: Regal Rexnord Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Regal Rexnord, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Regal Rexnord
provider_slug: regal-rexnord
slug: regal-rexnord-domain-security
source_filename: regal-rexnord-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.regalrexnord.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 22:25:57 2026 GMT\n  hsts: false\n- host: developer.regalrexnord.com\n  https: false\n- host: api.regalrexnord.com\n  https: false\ndomains:\n- domain: regalrexnord.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/regal-rexnord/refs/heads/main/security/regal-rexnord-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Industrial
- Motion Control
- Manufacturing
---
