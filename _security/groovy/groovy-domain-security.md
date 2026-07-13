---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: groovy-lang.org
  spf: false
hosts:
- cert_expires: Aug 22 11:15:29 2026 GMT
  host: groovy-lang.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Groovy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apache Groovy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Apache Groovy
provider_slug: groovy
slug: groovy-domain-security
source_filename: groovy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: groovy-lang.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 11:15:29 2026 GMT\n  hsts: false\ndomains:\n- domain: groovy-lang.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/groovy/refs/heads/main/security/groovy-domain-security.yml
summary_line: TLSv1.3
tags:
- Apache
- Dynamic Language
- JVM
- Programming Language
- Scripting
---
