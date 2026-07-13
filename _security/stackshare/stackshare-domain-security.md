---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: stackshare.io
  spf: true
hosts:
- cert_expires: Aug 12 19:52:50 2026 GMT
  host: stackshare.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: docs.stackshare.io
  https: false
- host: api.stackshare.io
  https: false
kind: domain-security
layout: security
method: probed
name: Stackshare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StackShare, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: StackShare
provider_slug: stackshare
slug: stackshare-domain-security
source_filename: stackshare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stackshare.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 19:52:50 2026 GMT\n  hsts: null\n- host: docs.stackshare.io\n  https: false\n- host: api.stackshare.io\n  https: false\ndomains:\n- domain: stackshare.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stackshare/refs/heads/main/security/stackshare-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Developer Tools
- Software Discovery
- Tech Stacks
---
