---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: colorful.app
  spf: true
hosts:
- cert_expires: Dec 19 11:21:39 2026 GMT
  host: colorful.app
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Colorful Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Colorful, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Colorful
provider_slug: colorful
slug: colorful-domain-security
source_filename: colorful-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: colorful.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 11:21:39 2026 GMT\n  hsts: false\ndomains:\n- domain: colorful.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/colorful/refs/heads/main/security/colorful-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
