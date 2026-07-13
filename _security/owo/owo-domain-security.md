---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: owo.vc
  spf: true
hosts:
- cert_expires: Sep 26 20:05:59 2026 GMT
  host: owo.vc
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Owo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for owo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: owo
provider_slug: owo
slug: owo-domain-security
source_filename: owo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: owo.vc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 20:05:59 2026 GMT\n  hsts: false\ndomains:\n- domain: owo.vc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/owo/refs/heads/main/security/owo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- URL Shorteners
- Public APIs
---
