---
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog"
  - 0 issuewild "entrust.com"
  - 0 issue "digicert.com"
  - 0 issue "sectigo.com"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: qt.io
  spf: true
hosts:
- cert_expires: Oct  4 07:36:37 2026 GMT
  host: www.qt.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Qt
provider_slug: qt
slug: qt-domain-security
source_filename: qt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.qt.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 07:36:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: qt.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"entrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qt/refs/heads/main/security/qt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Developer Tools
- Cross-Platform
- Framework
- SDK
- IDE
- Quality Assurance
- UI Design
- Embedded
---
