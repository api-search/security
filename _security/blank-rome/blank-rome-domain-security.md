---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: blankrome.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: blankromegr.com
  spf: true
hosts:
- cert_expires: Oct  6 08:35:26 2026 GMT
  host: www.blankrome.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 08:36:49 2026 GMT
  host: www.blankromegr.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blank Rome Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blank Rome LLP, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Blank Rome LLP
provider_slug: blank-rome
slug: blank-rome-domain-security
source_filename: blank-rome-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.blankrome.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 08:35:26 2026 GMT\n  hsts: null\n- host: www.blankromegr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 08:36:49 2026 GMT\n  hsts: false\ndomains:\n- domain: blankrome.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: blankromegr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blank-rome/refs/heads/main/security/blank-rome-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Am Law 100
- Corporate Law
- Government Affairs
- Government Contracts
- Intellectual Property
- Labor And Employment
- Law
- Law Firm
- Legal Services
- Litigation
- Lobbying
- Maritime Law
- Professional Services
- Restructuring
- Tax
- White Collar Defense
---
