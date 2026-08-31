---
description: TLS, HSTS and DNS posture for rapidsilicon.com, Rapid Silicon's registered corporate domain. The domain is still registered to the company through GoDaddy (registry expiry 2027-06-14) and its mail exchange still points at Microsoft 365 with a hard-fail SPF record and a DMARC policy, but since 2026-05-25 the web origin no longer serves company content. Absence of a record below is a measured observation, not an omission.
domains: []
hosts:
- dns:
    a:
    - 3.33.251.168
    - 15.197.225.128
    caa:
      note: no CAA record returned
      present: false
    dmarc:
      policy: quarantine
      present: true
      record: v=DMARC1; p=quarantine; pct=100
    dnssec:
      note: no DNSKEY record returned
      present: false
    mx:
    - rapidsilicon-com.mail.protection.outlook.com (priority 0)
    nameservers:
    - ns33.domaincontrol.com
    - ns34.domaincontrol.com
    spf:
      policy: hard fail (-all)
      present: true
      record: v=spf1 include:spf.protection.outlook.com -all
  host: rapidsilicon.com
  hsts:
    max_age: null
    present: false
  https:
    alpn: h2
    certificate_start_date: '2026-05-25'
    certificate_subject: CN=rapidsilicon.com
    cipher: AEAD-CHACHA20-POLY1305-SHA256
    note: GET / returns HTTP 301 to https://realdha.com/ (a third-party domain-for-sale page); HEAD / returns 405. All previously published product, blog and documentation paths return 404.
    reachable: true
    tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rapid Silicon Domain Security
name_suffix: Domain Security
overview: Domain security posture for Rapid Silicon, probed live across 1 host(s) and 0 registrable domain(s). 1 host(s) serve HTTPS; 1 advertise HSTS.
provider_name: Rapid Silicon
provider_slug: rapid-silicon
slug: rapid-silicon-domain-security
source_filename: rapid-silicon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: rapidsilicon.com (DNS + TLS probed directly 2026-08-26)\nname: Rapid Silicon domain security posture\ndescription: >-\n  TLS, HSTS and DNS posture for rapidsilicon.com, Rapid Silicon's registered corporate domain. The\n  domain is still registered to the company through GoDaddy (registry expiry 2027-06-14) and its mail\n  exchange still points at Microsoft 365 with a hard-fail SPF record and a DMARC policy, but since\n  2026-05-25 the web origin no longer serves company content. Absence of a record below is a measured\n  observation, not an omission.\nhosts:\n- host: rapidsilicon.com\n  https:\n    reachable: true\n    tls_version: TLSv1.3\n    cipher: AEAD-CHACHA20-POLY1305-SHA256\n    alpn: h2\n    certificate_subject: CN=rapidsilicon.com\n    certificate_start_date: '2026-05-25'\n    note: >-\n      GET / returns HTTP 301 to https://realdha.com/ (a third-party domain-for-sale page); HEAD /\n      returns 405. All previously\
  \ published product, blog and documentation paths return 404.\n  hsts:\n    present: false\n    max_age: null\n  dns:\n    a:\n    - 3.33.251.168\n    - 15.197.225.128\n    nameservers:\n    - ns33.domaincontrol.com\n    - ns34.domaincontrol.com\n    dnssec:\n      present: false\n      note: no DNSKEY record returned\n    caa:\n      present: false\n      note: no CAA record returned\n    spf:\n      present: true\n      record: v=spf1 include:spf.protection.outlook.com -all\n      policy: hard fail (-all)\n    dmarc:\n      present: true\n      record: v=DMARC1; p=quarantine; pct=100\n      policy: quarantine\n    mx:\n    - 'rapidsilicon-com.mail.protection.outlook.com (priority 0)'\nregistration:\n  registrar: GoDaddy.com, LLC\n  creation_date: '2019-06-14'\n  registry_expiry_date: '2027-06-14'\n  updated_date: '2026-05-25'\n  status:\n  - clientDeleteProhibited\n  - clientRenewProhibited\n  - clientTransferProhibited\n  - clientUpdateProhibited\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rapid-silicon/refs/heads/main/security/rapid-silicon-domain-security.yml
summary_line: HSTS
tags:
- Company
- Semiconductors
- FPGA
- eFPGA
- Electronic Design Automation
- Chip Design
- Open-Source
- Hardware
- Edge AI
- Silicon IP
---
