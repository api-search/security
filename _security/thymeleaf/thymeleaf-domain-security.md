---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: thymeleaf.org
  spf: false
hosts:
- cert_expires: Sep 23 11:48:22 2026 GMT
  host: www.thymeleaf.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thymeleaf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Thymeleaf, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Thymeleaf
provider_slug: thymeleaf
slug: thymeleaf-domain-security
source_filename: thymeleaf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thymeleaf.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 11:48:22 2026 GMT\n  hsts: false\ndomains:\n- domain: thymeleaf.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thymeleaf/refs/heads/main/security/thymeleaf-domain-security.yml
summary_line: TLSv1.3
tags:
- HTML
- Java
- Open Source
- Server Side Rendering
- Spring
- Spring Boot
- Template Engine
- Thymeleaf
- Web Development
---
