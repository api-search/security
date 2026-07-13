---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: qualys.com
  spf: true
hosts:
- cert_expires: Sep 30 18:41:52 2026 GMT
  host: www.qualys.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 18:41:52 2026 GMT
  host: docs.qualys.com
  hsts: true
  hsts_max_age: 63113904
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: qualysapi.qualys.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qualys Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qualys, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Qualys
provider_slug: qualys
slug: qualys-domain-security
source_filename: qualys-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.qualys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 18:41:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.qualys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 18:41:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63113904\n- host: qualysapi.qualys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: qualys.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qualys/refs/heads/main/security/qualys-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Security
- Vulnerability Management
- Compliance
- VMDR
- Cloud Security
- Web Application Scanning
---
