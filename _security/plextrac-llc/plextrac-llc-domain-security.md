---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: plextrac.com
  spf: true
hosts:
- cert_expires: Oct  2 20:44:32 2026 GMT
  host: plextrac.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 10:19:22 2026 GMT
  host: api-docs.plextrac.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 22:41:28 2026 GMT
  host: app.plextrac.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Plextrac Llc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PlexTrac, LLC, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PlexTrac, LLC
provider_slug: plextrac-llc
slug: plextrac-llc-domain-security
source_filename: plextrac-llc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: plextrac.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 20:44:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api-docs.plextrac.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 10:19:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.plextrac.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 22:41:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: plextrac.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plextrac-llc/refs/heads/main/security/plextrac-llc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cybersecurity
- Penetration Testing
- Vulnerability Management
- Security Reporting
- Exposure Management
- Offensive Security
- MSSP
- Remediation
---
