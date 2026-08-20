---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: monarchfts.com
  spf: true
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: core10.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getaccrue.com
  spf: true
hosts:
- cert_expires: Nov  6 14:14:37 2026 GMT
  host: monarchfts.com
  hsts: false
  https: true
  role: primary website (Core10 successor brand)
  tls_version: TLSv1.3
- cert_expires: Nov  5 23:39:55 2026 GMT
  host: core10.io
  hsts: false
  https: true
  role: retired Core10 domain, 301 to monarchfts.com
  tls_version: TLSv1.3
- cert_expires: Sep 20 21:47:03 2026 GMT
  host: blog.core10.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  role: Core10 Insights blog
  tls_version: TLSv1.3
- cert_expires: Oct 19 07:44:59 2026 GMT
  host: getaccrue.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  role: Accrue product site
  tls_version: TLSv1.3
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: api.getaccrue.com
  hsts: false
  https: true
  role: Accrue API host (live nginx, no public contract)
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Core10 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Core10, probed live across 5 host(s) and 3 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Core10
provider_slug: core10
slug: core10-domain-security
source_filename: core10-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of every Core10-lineage host\nnote: >-\n  Core10's own domain, core10.io, still holds a valid certificate and 301-redirects to\n  monarchfts.com. api.getaccrue.com is the only live API host in the lineage; it is the\n  weakest posture here — TLSv1.2 and no HSTS header at all — and it serves a bare nginx 404\n  on every path, so nothing about the contract behind it is public.\nhosts:\n- host: monarchfts.com\n  role: primary website (Core10 successor brand)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 14:14:37 2026 GMT\n  hsts: false\n- host: core10.io\n  role: retired Core10 domain, 301 to monarchfts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:39:55 2026 GMT\n  hsts: false\n- host: blog.core10.io\n  role: Core10 Insights blog\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 21:47:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: getaccrue.com\n\
  \  role: Accrue product site\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 07:44:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.getaccrue.com\n  role: Accrue API host (live nginx, no public contract)\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: monarchfts.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: core10.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: getaccrue.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\nx-evidence:\n  fetched: '2026-08-11'\n  hosts_probed: 5\n  domains_probed: 3\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/core10/refs/heads/main/security/core10-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Financial-Services
- Banking
- API Integration
- Software Development
- Digital Lending
- Account Opening
- Salesforce
- Consulting
- Professional Services
- Private Capital
- Tennessee
---
