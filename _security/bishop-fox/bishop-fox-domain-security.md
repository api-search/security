---
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bishopfox.com
  spf: true
hosts:
- cert_expires: Oct  6 22:20:51 2026 GMT
  host: bishopfox.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 23:59:59 2026 GMT
  host: cosmos.bishopfox.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: api.cosmos.bishopfox.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bishop Fox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bishop Fox, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Bishop Fox
provider_slug: bishop-fox
slug: bishop-fox-domain-security
source_filename: bishop-fox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bishopfox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 22:20:51 2026 GMT\n  hsts: false\n- host: cosmos.bishopfox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.cosmos.bishopfox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: bishopfox.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bishop-fox/refs/heads/main/security/bishop-fox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cybersecurity
- Offensive Security
- Penetration Testing
- Attack Surface Management
- Exposure Management
- Red Teaming
- Vulnerability Management
- Security Findings
- Asset Discovery
- Continuous Threat Exposure Management
- Authentication
---
