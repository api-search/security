---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zube.io
  spf: true
hosts:
- cert_expires: Aug 31 03:09:07 2026 GMT
  host: zube.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zube Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zube, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zube
provider_slug: zube
slug: zube-domain-security
source_filename: zube-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zube.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 03:09:07 2026 GMT\n  hsts: false\ndomains:\n- domain: zube.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zube/refs/heads/main/security/zube-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Documents And Productivity
- Public APIs
---
