---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jakarta.ee
  spf: false
hosts:
- cert_expires: Sep 25 01:24:39 2026 GMT
  host: jakarta.ee
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jpa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JPA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: JPA
provider_slug: jpa
slug: jpa-domain-security
source_filename: jpa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jakarta.ee\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 01:24:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jakarta.ee\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jpa/refs/heads/main/security/jpa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Database
- Java
- JPA
- Jakarta EE
- ORM
- Persistence
---
