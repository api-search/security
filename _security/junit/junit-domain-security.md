---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: junit.org
  spf: true
hosts:
- cert_expires: Oct  3 02:04:52 2026 GMT
  host: junit.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Junit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JUnit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: JUnit
provider_slug: junit
slug: junit-domain-security
source_filename: junit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: junit.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 02:04:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: junit.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/junit/refs/heads/main/security/junit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Java
- TDD
- Test Automation
- Testing
- Unit Testing
---
