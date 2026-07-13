---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cucumber.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: specflow.org
  spf: false
hosts:
- cert_expires: Sep 19 21:36:15 2026 GMT
  host: cucumber.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: specflow.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 13:13:23 2026 GMT
  host: behave.readthedocs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bdd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BDD (Behavior-Driven Development), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BDD (Behavior-Driven Development)
provider_slug: bdd
slug: bdd-domain-security
source_filename: bdd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cucumber.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 21:36:15 2026 GMT\n  hsts: false\n- host: specflow.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: behave.readthedocs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 13:13:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cucumber.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: specflow.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bdd/refs/heads/main/security/bdd-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automation
- BDD
- Software Development
- Testing
- Gherkin
- Quality Assurance
---
