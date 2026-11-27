---
description: ''
domains:
- caa:
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: parallaxprotocol.org
  spf: true
hosts:
- cert_expires: Jan  4 11:35:58 2027 GMT
  host: parallaxprotocol.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Parallax Protocol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parallax Protocol, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Parallax Protocol
provider_slug: parallaxprotocol-org
slug: parallaxprotocol-org-domain-security
source_filename: parallaxprotocol-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: parallaxprotocol.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 11:35:58 2027 GMT\n  hsts: false\ndomains:\n- domain: parallaxprotocol.org\n  dnssec: true\n  caa:\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/parallaxprotocol-org/security/parallaxprotocol-org-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Blockchain
- Cryptocurrency
- Open Source
- Decentralized
- Finance
---
