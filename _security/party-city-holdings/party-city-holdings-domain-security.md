---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: partycity.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: party-city-holdings.com
  spf: false
hosts:
- cert_expires: Sep 24 10:00:23 2026 GMT
  host: www.partycity.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
- host: www.party-city-holdings.com
  https: false
kind: domain-security
layout: security
method: probed
name: Party City Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Party City Holdings, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Party City Holdings
provider_slug: party-city-holdings
slug: party-city-holdings-domain-security
source_filename: party-city-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.partycity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 10:00:23 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: www.party-city-holdings.com\n  https: false\ndomains:\n- domain: partycity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: party-city-holdings.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/party-city-holdings/refs/heads/main/security/party-city-holdings-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Retail
- Party Supplies
- E-commerce
---
