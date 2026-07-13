---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cucumber.io
  spf: true
hosts:
- cert_expires: Sep 19 21:36:15 2026 GMT
  host: cucumber.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cucumber Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cucumber, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cucumber
provider_slug: cucumber
slug: cucumber-domain-security
source_filename: cucumber-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cucumber.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 21:36:15 2026 GMT\n  hsts: false\ndomains:\n- domain: cucumber.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cucumber/refs/heads/main/security/cucumber-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Automation
- BDD
- Behavior Driven Development
- Gherkin
- Open Source
- Quality Assurance
- Test Framework
- Testing
---
