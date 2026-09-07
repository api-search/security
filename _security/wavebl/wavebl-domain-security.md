---
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wavebl.com
  spf: true
hosts:
- cert_expires: Oct 28 16:23:11 2026 GMT
  host: wavebl.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: coa.wavebl.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Wavebl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WaveBL, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: WaveBL
provider_slug: wavebl
slug: wavebl-domain-security
source_filename: wavebl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wavebl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 16:23:11 2026 GMT\n  hsts: false\n- host: coa.wavebl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: wavebl.com\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wavebl/refs/heads/main/security/wavebl-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Electronic Bill of Lading
- Digital Trade
- Trade Documents
- Trade Finance
- Ocean Freight
- Shipping
- Logistics
- Supply Chain
- Maritime
- Customs
- Blockchain
- Freight Forwarding
- Banking
- Document Exchange
---
