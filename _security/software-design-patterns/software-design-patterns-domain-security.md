---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: refactoring.guru
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: patterns.dev
  spf: false
hosts:
- cert_expires: Sep 12 01:42:36 2026 GMT
  host: refactoring.guru
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 03:50:39 2026 GMT
  host: www.patterns.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Software Design Patterns Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Software Design Patterns, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Software Design Patterns
provider_slug: software-design-patterns
slug: software-design-patterns-domain-security
source_filename: software-design-patterns-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: refactoring.guru\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 01:42:36 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: www.patterns.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 03:50:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: refactoring.guru\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: patterns.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/software-design-patterns/refs/heads/main/security/software-design-patterns-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Architecture
- Best Practices
- Object-Oriented Programming
- Software Engineering
- Design Patterns
- Gang of Four
- Creational Patterns
- Structural Patterns
- Behavioral Patterns
---
