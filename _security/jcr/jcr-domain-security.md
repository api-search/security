---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  dmarc: false
  dnssec: false
  domain: jcp.org
  spf: true
hosts:
- cert_expires: Sep 17 23:59:59 2026 GMT
  host: jcp.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jcr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JCR, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: JCR
provider_slug: jcr
slug: jcr-domain-security
source_filename: jcr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jcp.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jcp.org\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jcr/refs/heads/main/security/jcr-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- CMS
- Content Repository
- Java
- JCR
- JSR-283
- Standard
---
