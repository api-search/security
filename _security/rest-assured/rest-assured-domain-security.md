---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: rest-assured.io
  spf: true
hosts:
- cert_expires: Sep 28 04:49:50 2026 GMT
  host: rest-assured.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rest Assured Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for REST Assured, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: REST Assured
provider_slug: rest-assured
slug: rest-assured-domain-security
source_filename: rest-assured-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rest-assured.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 04:49:50 2026 GMT\n  hsts: false\ndomains:\n- domain: rest-assured.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rest-assured/refs/heads/main/security/rest-assured-domain-security.yml
summary_line: TLSv1.3
tags:
- Functional Testing
- Testing
- Java
- API Testing
- Automation
---
