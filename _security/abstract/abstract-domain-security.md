---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: goabstract.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: abstract.com
  spf: true
hosts:
- cert_expires: Sep 23 23:48:08 2026 GMT
  host: www.goabstract.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.abstract.com
  https: false
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: api.goabstract.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Abstract Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Abstract, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Abstract
provider_slug: abstract
slug: abstract-domain-security
source_filename: abstract-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.goabstract.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:48:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.abstract.com\n  https: false\n- host: api.goabstract.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: goabstract.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: abstract.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abstract/refs/heads/main/security/abstract-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Design
- Version Control
- Collaboration
- Sketch
- Design Systems
---
