---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: jmock.org
  spf: false
hosts:
- cert_expires: Sep 14 17:24:51 2026 GMT
  host: www.jmock.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jmock Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JMock, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: JMock
provider_slug: jmock
slug: jmock-domain-security
source_filename: jmock-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jmock.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 17:24:51 2026 GMT\n  hsts: false\ndomains:\n- domain: jmock.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jmock/refs/heads/main/security/jmock-domain-security.yml
summary_line: TLSv1.3
tags:
- Java
- Mock Objects
- Mocking
- TDD
- Testing
- Unit Testing
---
