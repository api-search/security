---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mockito.org
  spf: false
hosts:
- cert_expires: Sep 24 08:52:49 2026 GMT
  host: site.mockito.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mockito Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mockito, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Mockito
provider_slug: mockito
slug: mockito-domain-security
source_filename: mockito-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: site.mockito.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 08:52:49 2026 GMT\n  hsts: false\ndomains:\n- domain: mockito.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mockito/refs/heads/main/security/mockito-domain-security.yml
summary_line: TLSv1.3
tags:
- Java
- Mocking
- Testing
- Unit Testing
- Open Source
- Framework
---
