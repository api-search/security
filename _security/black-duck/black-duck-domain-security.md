---
description: ''
domains:
- caa:
  - 0 issue "entrust.net"
  - 0 issue "amazonaws.com"
  - 0 issue "digicert.com"
  - 0 issuewild "sectigo.com"
  - 0 issue "pki.goog"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: blackduck.com
  spf: true
hosts:
- cert_expires: Sep 13 20:06:32 2026 GMT
  host: documentation.blackduck.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 23:59:59 2026 GMT
  host: polaris.blackduck.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Black Duck Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Black Duck, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Black Duck
provider_slug: black-duck
slug: black-duck-domain-security
source_filename: black-duck-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: documentation.blackduck.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 20:06:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: polaris.blackduck.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: blackduck.com\n  dnssec: false\n  caa:\n  - 0 issue \"entrust.net\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/black-duck/refs/heads/main/security/black-duck-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Application Security
- Software Composition Analysis
- SAST
- DAST
- Open Source Security
- DevSecOps
- Vulnerability Management
---
