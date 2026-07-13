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
- cert_expires: Aug 19 06:54:45 2026 GMT
  host: docs.sourcehut.org
  hsts: false
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
name: Sourcehut Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SourceHut, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SourceHut
provider_slug: sourcehut
slug: sourcehut-domain-security
source_filename: sourcehut-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sourcehut.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 16:04:34 2026 GMT\n  hsts: false\n- host: docs.sourcehut.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 06:54:45 2026 GMT\n  hsts: false\n- host: git.sr.ht\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 00:01:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sourcehut.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: sr.ht\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sourcehut/refs/heads/main/security/sourcehut-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Git
- Mercurial
- Source Control
- Continuous Integration
- Mailing Lists
- Issue Tracking
- Developer Tools
- Open Source
- Privacy
- GraphQL
---
