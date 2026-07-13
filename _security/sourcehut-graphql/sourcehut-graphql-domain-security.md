---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sourcehut.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sr.ht
  spf: true
hosts:
- cert_expires: Sep 13 16:04:34 2026 GMT
  host: sourcehut.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 19:16:50 2026 GMT
  host: man.sr.ht
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 00:01:40 2026 GMT
  host: git.sr.ht
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sourcehut Graphql Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sourcehut GraphQL, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sourcehut GraphQL
provider_slug: sourcehut-graphql
slug: sourcehut-graphql-domain-security
source_filename: sourcehut-graphql-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sourcehut.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 16:04:34 2026 GMT\n  hsts: false\n- host: man.sr.ht\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 19:16:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: git.sr.ht\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 00:01:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sourcehut.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: sr.ht\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sourcehut-graphql/refs/heads/main/security/sourcehut-graphql-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- GraphQL
- Developer Tools
- Software Forge
- Version Control
- Open Source
- CI/CD
- Git
---
