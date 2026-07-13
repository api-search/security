---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: oasdiff.com
  spf: true
hosts:
- cert_expires: Aug 18 06:34:54 2026 GMT
  host: www.oasdiff.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oasdiff Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oasdiff, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Oasdiff
provider_slug: oasdiff
slug: oasdiff-domain-security
source_filename: oasdiff-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.oasdiff.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 06:34:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: oasdiff.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oasdiff/refs/heads/main/security/oasdiff-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Breaking Changes
- Changelogs
- Deprecation
- OpenAPI
---
