---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wired.com
  spf: true
hosts:
- cert_expires: Oct  7 19:34:15 2026 GMT
  host: www.wired.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wired Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wired, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Wired
provider_slug: wired
slug: wired-domain-security
source_filename: wired-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wired.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 19:34:15 2026 GMT\n  hsts: false\ndomains:\n- domain: wired.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wired/refs/heads/main/security/wired-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Content
- Innovation
- Media
- News
- RSS
- Science
- Technology News
---
