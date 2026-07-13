---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:devops@softwareadvice.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: softwareadvice.com
  spf: true
hosts:
- cert_expires: Oct  5 15:21:36 2026 GMT
  host: www.softwareadvice.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Software Advice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Software Advice, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Software Advice
provider_slug: software-advice
slug: software-advice-domain-security
source_filename: software-advice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.softwareadvice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 15:21:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: softwareadvice.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:devops@softwareadvice.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/software-advice/refs/heads/main/security/software-advice-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- B2B
- Software Recommendations
- Software Reviews
- Analytics
- Gartner
---
