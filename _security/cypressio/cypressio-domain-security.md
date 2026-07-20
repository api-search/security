---
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cypress.io
  spf: true
hosts:
- cert_expires: Sep  6 22:58:24 2026 GMT
  host: docs.cypress.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 22:58:24 2026 GMT
  host: cloud.cypress.io
  hsts: true
  hsts_max_age: 631138519
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cypressio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cypress.io, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cypress.io
provider_slug: cypressio
slug: cypressio-domain-security
source_filename: cypressio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.cypress.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 22:58:24 2026 GMT\n  hsts: false\n- host: cloud.cypress.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 22:58:24 2026 GMT\n  hsts: true\n  hsts_max_age: 631138519\ndomains:\n- domain: cypress.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cypressio/refs/heads/main/security/cypressio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Testing
- End-to-End Testing
- Test Automation
- Quality Assurance
- Developer Tools
- CI/CD
- Accessibility
- JavaScript
---
