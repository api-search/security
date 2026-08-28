---
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: maymaan.com
  spf: true
hosts:
- cert_expires: Oct 29 07:07:46 2026 GMT
  host: maymaan.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Maymaan Research Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MayMaan Research, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MayMaan Research
provider_slug: maymaan-research
slug: maymaan-research-domain-security
source_filename: maymaan-research-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: maymaan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 07:07:46 2026 GMT\n  hsts: false\ndomains:\n- domain: maymaan.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nnotes:\n- >-\n  The TLS certificate served for maymaan.com carries a single subjectAltName\n  (DNS:maymaan.com) and does NOT cover www.maymaan.com. A request to\n  https://www.maymaan.com/ fails certificate verification outright\n  (\"no alternative certificate subject name matches target host name\"), so the\n  www hostname is unreachable over HTTPS. Observed 2026-08-25 via\n  `openssl s_client -servername www.maymaan.com`. The\
  \ apex host is healthy\n  (TLSv1.3, valid cert). All pointers in apis.yml therefore use the apex host.\n- >-\n  No HSTS header is served on the apex host, and the registrable domain has no\n  DNSSEC. SPF and DMARC are both published (DMARC p=quarantine), and CAA records\n  are set, restricting issuance to six named CAs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maymaan-research/refs/heads/main/security/maymaan-research-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Energy
- Clean Energy
- Power Generation
- Engines
- Manufacturing
- Hardware
- Sustainability
- Data Centers
- Automotive
---
