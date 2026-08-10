---
description: ''
domains:
- caa: []
  dmarc: false
  dns_status: NOERROR-NODATA
  dnssec: false
  domain: dunzo.com
  https: false
  nameservers:
  - DNS1.BIGROCK.IN
  - DNS2.BIGROCK.IN
  - DNS3.BIGROCK.IN
  - DNS4.BIGROCK.IN
  registrant_organization: Domains By Proxy, LLC
  registrar: GoDaddy.com, LLC
  resolves: false
  spf: false
  whois_expires: '2028-01-26'
  whois_updated: '2026-02-24'
- caa: []
  dmarc: false
  dns_status: SERVFAIL
  dnssec: false
  domain: dunzo.in
  https: false
  resolves: false
  spf: false
hosts: []
kind: domain-security
layout: security
method: probed
name: Dunzo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dunzo, probed live across 0 host(s) and 2 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Dunzo
provider_slug: dunzo
slug: dunzo-domain-security
source_filename: dunzo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the Dunzo registrable domains\nnote: >-\n  Dunzo was dissolved on 2025-01-14 and its app and website were shut down. No Dunzo-operated\n  host resolves. dunzo.com answers NOERROR/NODATA (registry delegation to BigRock nameservers,\n  registrant now the privacy proxy \"Domains By Proxy, LLC\" as of the 2026-02-24 whois update) and\n  serves no A, AAAA, MX, TXT, CAA or DS record; dunzo.in delegation is broken (SERVFAIL). There is\n  therefore no TLS, HSTS, SPF or DMARC posture to measure. The earlier automated run of\n  0-working/probe-domain-security.py measured forgeglobal.com — the third-party secondary-market\n  listing host recorded as the harvest source — which is not a Dunzo host; that result was removed\n  as a misattribution.\nhosts: []\ndomains:\n- domain: dunzo.com\n  resolves: false\n  dns_status: NOERROR-NODATA\n  https: false\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n \
  \ registrar: GoDaddy.com, LLC\n  registrant_organization: Domains By Proxy, LLC\n  nameservers:\n  - DNS1.BIGROCK.IN\n  - DNS2.BIGROCK.IN\n  - DNS3.BIGROCK.IN\n  - DNS4.BIGROCK.IN\n  whois_updated: '2026-02-24'\n  whois_expires: '2028-01-26'\n- domain: dunzo.in\n  resolves: false\n  dns_status: SERVFAIL\n  https: false\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\nx-evidence:\n- probed: '2026-08-04'\n  check: dig A/AAAA/NS/MX/TXT/CAA/DS dunzo.com\n  result: NOERROR with no answer records\n- probed: '2026-08-04'\n  check: dig NS dunzo.in\n  result: SERVFAIL (broken delegation)\n- probed: '2026-08-04'\n  check: curl https://dunzo.com/ (and www., api., apis.dunzo.in, developers., docs., business.)\n  result: 'curl (6) could not resolve host — every candidate host'\n- probed: '2026-08-04'\n  check: whois dunzo.com\n  result: registrant is Domains By Proxy, LLC; nameservers BigRock; updated 2026-02-24\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dunzo/refs/heads/main/security/dunzo-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Delivery
- Last Mile Delivery
- Hyperlocal
- Quick Commerce
- Logistics
- E-Commerce
- India
- Defunct
---
