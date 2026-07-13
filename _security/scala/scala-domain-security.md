---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: scala-lang.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: akka.io
  spf: true
hosts:
- cert_expires: Aug 12 07:56:31 2026 GMT
  host: www.scala-lang.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 15:03:40 2026 GMT
  host: doc.akka.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 01:53:33 2026 GMT
  host: www.playframework.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scala Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scala, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Scala
provider_slug: scala
slug: scala-domain-security
source_filename: scala-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.scala-lang.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 07:56:31 2026 GMT\n  hsts: false\n- host: doc.akka.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 15:03:40 2026 GMT\n  hsts: false\n- host: www.playframework.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 01:53:33 2026 GMT\n  hsts: false\ndomains:\n- domain: scala-lang.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: akka.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scala/refs/heads/main/security/scala-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Big Data
- Distributed Systems
- Functional Programming
- JVM
- Programming Language
- Scala
- Scala 3
- Type Safety
---
