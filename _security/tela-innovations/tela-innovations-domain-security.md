---
description: 'Domain and transport security posture for the one host Tela Innovations, Inc. still holds, tela-inc.com. Absence of a record is valid data and is recorded as such. Note that this domain no longer serves a website: TLS could not be assessed because port 443 does not accept connections.'
domains: []
hosts:
- a_record: 129.121.136.207
  host: tela-inc.com
  hsts:
    max_age: null
    note: Not assessable — no HTTP response to read headers from.
    present: false
  http:
    port_80: closed
    reachable: false
  https:
    certificate_expires: null
    note: TCP connection to 129.121.136.207:443 is refused/times out, so no TLS handshake is possible and no certificate could be read.
    port_443: closed
    reachable: false
    tls_version: null
  registrable_domain: tela-inc.com
- a_record: 129.121.136.207
  host: www.tela-inc.com
  hsts:
    max_age: null
    present: false
  http:
    port_80: closed
    reachable: false
  https:
    certificate_expires: null
    port_443: closed
    reachable: false
    tls_version: null
  registrable_domain: tela-inc.com
kind: domain-security
layout: security
method: probed
name: Tela Innovations Domain Security
name_suffix: Domain Security
overview: Domain security posture for Tela Innovations, probed live across 2 host(s) and 0 registrable domain(s). 2 host(s) serve HTTPS; 2 advertise HSTS.
provider_name: Tela Innovations
provider_slug: tela-innovations
slug: tela-innovations-domain-security
source_filename: tela-innovations-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: tela-inc.com (DNS + TCP + WHOIS probe, 2026-08-29)\nname: Tela Innovations domain security posture\ndescription: >-\n  Domain and transport security posture for the one host Tela Innovations, Inc. still holds,\n  tela-inc.com. Absence of a record is valid data and is recorded as such. Note that this domain\n  no longer serves a website: TLS could not be assessed because port 443 does not accept\n  connections.\n\nhosts:\n- host: tela-inc.com\n  registrable_domain: tela-inc.com\n  a_record: 129.121.136.207\n  https:\n    reachable: false\n    port_443: closed\n    tls_version: null\n    certificate_expires: null\n    note: >-\n      TCP connection to 129.121.136.207:443 is refused/times out, so no TLS handshake is\n      possible and no certificate could be read.\n  http:\n    reachable: false\n    port_80: closed\n  hsts:\n    present: false\n    max_age: null\n    note: Not assessable — no HTTP response to read headers from.\n\
  - host: www.tela-inc.com\n  registrable_domain: tela-inc.com\n  a_record: 129.121.136.207\n  https:\n    reachable: false\n    port_443: closed\n    tls_version: null\n    certificate_expires: null\n  http:\n    reachable: false\n    port_80: closed\n  hsts:\n    present: false\n    max_age: null\n\ndns:\n  registrable_domain: tela-inc.com\n  nameservers:\n  - ns1.no-ip.com\n  - ns2.no-ip.com\n  - ns3.no-ip.com\n  - ns4.no-ip.com\n  - ns5.no-ip.com\n  dnssec:\n    present: false\n    dnskey_records: 0\n  caa:\n    present: false\n    records: []\n    note: No CAA record — any public CA may issue for this domain.\n  spf:\n    present: false\n    records: []\n    note: >-\n      No TXT record of any kind is published at the apex, so there is no SPF policy. Mail is\n      routed to Microsoft 365 (MX 5 telainc-com01b.mail.eo.outlook.com) with no sender\n      authentication published.\n  dmarc:\n    present: false\n    record: null\n    policy: null\n    note: No _dmarc.tela-inc.com TXT record.\n\
  \  mx:\n  - preference: 5\n    exchange: telainc-com01b.mail.eo.outlook.com\n\nregistration:\n  registrar: Vitalwerks Internet Solutions, LLC / No-IP.com\n  created: '2005-12-20'\n  updated: '2022-12-01'\n  expires: '2026-12-20'\n  status:\n  - clientTransferProhibited\n\nfindings:\n- The domain is registered and renewed, and mail still routes to Microsoft 365, so the name has\n  not been abandoned or reassigned to a third party.\n- No web service runs on it. Both port 80 and port 443 refuse connections, so there is no site,\n  no docs, no developer portal and no TLS posture to assess.\n- No SPF, no DMARC, no CAA and no DNSSEC are published, which is a live risk for a domain that\n  still receives mail — the name remains spoofable.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tela-innovations/refs/heads/main/security/tela-innovations-domain-security.yml
summary_line: HSTS
tags:
- Company
- Semiconductors
- Electronic Design Automation
- Chip Design
- Intellectual Property
- Standard Cell Libraries
- Design For Manufacturing
- Patent Licensing
- Defunct
---
