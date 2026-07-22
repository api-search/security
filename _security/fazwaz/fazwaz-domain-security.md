---
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fazwaz.com
  spf: true
hosts:
- cert_expires: Aug 21 09:17:18 2026 GMT
  host: fazwaz.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fazwaz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FazWaz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FazWaz
provider_slug: fazwaz
slug: fazwaz-domain-security
source_filename: fazwaz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fazwaz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 09:17:18 2026 GMT\n  hsts: false\ndomains:\n- domain: fazwaz.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fazwaz/refs/heads/main/security/fazwaz-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Real Estate
- PropTech
- Property Listings
- Marketplace
- Thailand
- Southeast Asia
- GraphQL
---
