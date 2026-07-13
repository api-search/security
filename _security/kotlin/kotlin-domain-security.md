---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild ";"
  - 0 iodef "mailto:caa-iodef@jetbrains.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kotlinlang.org
  spf: true
hosts:
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: kotlinlang.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kotlin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kotlin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kotlin
provider_slug: kotlin
slug: kotlin-domain-security
source_filename: kotlin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kotlinlang.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: kotlinlang.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \";\"\n  - 0 iodef \"mailto:caa-iodef@jetbrains.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kotlin/refs/heads/main/security/kotlin-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Android
- JVM
- Kotlin
- Multiplatform
- Programming Language
---
