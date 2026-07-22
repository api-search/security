---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "geotrust.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kodiaknetworks.com
  spf: true
hosts:
- host: www.kodiaknetworks.com
  https: false
kind: domain-security
layout: security
method: probed
name: Kodiak Networks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kodiak Networks, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kodiak Networks
provider_slug: kodiak-networks
slug: kodiak-networks-domain-security
source_filename: kodiak-networks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kodiaknetworks.com\n  https: false\ndomains:\n- domain: kodiaknetworks.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"geotrust.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kodiak-networks/refs/heads/main/security/kodiak-networks-domain-security.yml
summary_line: DMARC
tags:
- Company
- Push To Talk
- Telecommunications
- Mobile
- Public Safety
- Wireless Carriers
- MCPTT
- Acquired
---
