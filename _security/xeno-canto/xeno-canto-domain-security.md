---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: xeno-canto.org
  spf: true
hosts:
- cert_expires: Sep 29 19:11:33 2026 GMT
  host: xeno-canto.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Xeno Canto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for xeno-canto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: xeno-canto
provider_slug: xeno-canto
slug: xeno-canto-domain-security
source_filename: xeno-canto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xeno-canto.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 19:11:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: xeno-canto.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xeno-canto/refs/heads/main/security/xeno-canto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Animals
- Public APIs
---
