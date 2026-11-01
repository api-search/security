---
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 iodef "sectigo.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: rtx.com
  spf: true
hosts:
- cert_expires: Nov 29 10:36:16 2026 GMT
  host: www.rtx.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Raytheonintelligenceandspace Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BBN, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: BBN
provider_slug: raytheonintelligenceandspace-com
slug: raytheonintelligenceandspace-com-domain-security
source_filename: raytheonintelligenceandspace-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rtx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 10:36:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: rtx.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"sectigo.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/raytheonintelligenceandspace-com/security/raytheonintelligenceandspace-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Defense
- Communications
- Cybersecurity
- SignalProcessing
---
