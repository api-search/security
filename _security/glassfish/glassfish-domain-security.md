---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: glassfish.org
  spf: false
hosts:
- cert_expires: Sep 16 15:38:23 2026 GMT
  host: glassfish.org
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Glassfish Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eclipse GlassFish, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Eclipse GlassFish
provider_slug: glassfish
slug: glassfish-domain-security
source_filename: glassfish-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: glassfish.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 15:38:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: glassfish.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glassfish/refs/heads/main/security/glassfish-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Application Server
- Jakarta EE
- Java EE
- Open Source
- Eclipse Foundation
- Servlet Container
- Reference Implementation
---
