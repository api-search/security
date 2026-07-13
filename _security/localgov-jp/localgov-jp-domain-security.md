---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: localgov.jp
  spf: true
hosts:
- cert_expires: Oct  1 00:44:04 2026 GMT
  host: localgov.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Localgov Jp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LocalGov.jp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: LocalGov.jp
provider_slug: localgov-jp
slug: localgov-jp-domain-security
source_filename: localgov-jp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: localgov.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 00:44:04 2026 GMT\n  hsts: false\ndomains:\n- domain: localgov.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/localgov-jp/refs/heads/main/security/localgov-jp-domain-security.yml
summary_line: TLSv1.3
tags:
- Government
- Public APIs
---
