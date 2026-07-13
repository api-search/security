---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: nunit.org
  spf: true
hosts:
- cert_expires: Sep 27 23:58:26 2026 GMT
  host: nunit.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 18:17:18 2026 GMT
  host: docs.nunit.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nunit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NUnit, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: NUnit
provider_slug: nunit
slug: nunit-domain-security
source_filename: nunit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nunit.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 23:58:26 2026 GMT\n  hsts: false\n- host: docs.nunit.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 18:17:18 2026 GMT\n  hsts: false\ndomains:\n- domain: nunit.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nunit/refs/heads/main/security/nunit-domain-security.yml
summary_line: TLSv1.3
tags:
- .NET
- C#
- Framework
- Open Source
- TDD
- Testing
- Unit Testing
---
