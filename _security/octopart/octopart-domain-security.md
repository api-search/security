---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: octopart.com
  spf: true
hosts:
- cert_expires: Aug 16 15:14:11 2026 GMT
  host: octopart.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Octopart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Octopart, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Octopart
provider_slug: octopart
slug: octopart-domain-security
source_filename: octopart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: octopart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 15:14:11 2026 GMT\n  hsts: null\ndomains:\n- domain: octopart.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/octopart/refs/heads/main/security/octopart-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Shopping
- Public APIs
---
