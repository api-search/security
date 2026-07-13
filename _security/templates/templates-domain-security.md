---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: handlebarsjs.com
  spf: false
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security@palletsprojects.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: false
  dnssec: false
  domain: palletsprojects.com
  spf: true
hosts:
- cert_expires: Sep 19 09:41:54 2026 GMT
  host: handlebarsjs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 13:39:26 2026 GMT
  host: jinja.palletsprojects.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 11:13:19 2026 GMT
  host: openapi-generator.tech
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Templates Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Templates, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Templates
provider_slug: templates
slug: templates-domain-security
source_filename: templates-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: handlebarsjs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 09:41:54 2026 GMT\n  hsts: false\n- host: jinja.palletsprojects.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 13:39:26 2026 GMT\n  hsts: false\n- host: openapi-generator.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 11:13:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: handlebarsjs.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: palletsprojects.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security@palletsprojects.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/templates/refs/heads/main/security/templates-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Templates
- API Design
- Code Generation
- Documentation
- OpenAPI
- AsyncAPI
---
