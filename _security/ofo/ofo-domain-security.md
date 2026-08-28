---
description: ''
domains: []
hosts:
- host: ofo.com
  hsts: null
  https: false
  note: The A record resolves (47.93.164.86, Aliyun) and the registration is live through Alibaba Cloud to 2027-09-08, but the origin completes no TCP handshake on either web port, so TLS, HSTS and certificate posture cannot be observed at all — the web presence is off, not merely misconfigured.
  ports:
    '443': closed
    '80': closed
  reachable: false
  tls_version: null
kind: domain-security
layout: security
method: probed
name: Ofo Domain Security
name_suffix: Domain Security
overview: Domain security posture for Ofo, probed live across 1 host(s) and 0 registrable domain(s).
provider_name: Ofo
provider_slug: ofo
slug: ofo-domain-security
source_filename: ofo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  Direct TCP/TLS probe of 47.93.164.86 (ofo.com) plus DNS queries against 8.8.8.8 for TXT, MX,\n  CAA, DS and DNSKEY on ofo.com.\nscope: >-\n  ofo.com only — the company's own former primary host. forgeglobal.com, which is currently the\n  only URL in apis.yml common[], is a third-party secondary-market trading venue; its security\n  posture is Forge Global's and is deliberately NOT probed or attributed to Ofo here.\npointer_emitted: false\npointer_note: >-\n  No `DomainSecurity` (or `Security`) pointer is wired into apis.yml for this file. The scorer's\n  `reg_security_posture` check awards points for the pointer alone, and Ofo publishes no security\n  posture — every control below is absent and the web origin is offline. Wiring a pointer here\n  would convert a verified absence into a scored presence.\nhosts:\n- host: ofo.com\n  reachable: false\n  ports:\n    '80': closed\n    '443': closed\n  https: false\n  tls_version:\
  \ null\n  hsts: null\n  note: >-\n    The A record resolves (47.93.164.86, Aliyun) and the registration is live through Alibaba\n    Cloud to 2027-09-08, but the origin completes no TCP handshake on either web port, so TLS,\n    HSTS and certificate posture cannot be observed at all — the web presence is off, not merely\n    misconfigured.\ndns:\n  registrable_domain: ofo.com\n  dnssec:\n    enabled: false\n    ds: []\n    dnskey: []\n  caa:\n    present: false\n    records: []\n  spf:\n    present: true\n    valid: false\n    records:\n    - v=spf1 include:spf.163.com -all\n    - v=spf1 include:spf.corp-email.com include:spfb.corp-email.com ~all\n    note: >-\n      TWO v=spf1 TXT records are published on the same name. RFC 7208 §4.5 makes that a\n      permanent error — a receiver that finds more than one SPF record MUST return permerror,\n      so in practice this domain has no usable SPF policy despite publishing two.\n  dmarc:\n    present: false\n    record: null\n  mx:\n  - 5 hzmx01.mxmail.netease.com\n\
  \  - 10 hzmx02.mxmail.netease.com\n  other_txt:\n  - MS=ms74974185\n  note: >-\n    Corporate mail is still delegated to NetEase business mail and the domain is still being\n    renewed, so the registration is administered even though the website is gone. Mail\n    authentication is nonetheless unusable: conflicting SPF records and no DMARC record at all.\nx-evidence:\n  fetched: '2026-08-26'\n  probes:\n  - url: https://ofo.com/\n    status: 0\n  - url: http://ofo.com/\n    status: 0\n  - url: https://www.ofo.com/\n    status: 0\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ofo/refs/heads/main/security/ofo-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Defunct
- Transportation
- Mobility
- Micromobility
- Bike Sharing
- Sharing Economy
- Consumer
- China
---
