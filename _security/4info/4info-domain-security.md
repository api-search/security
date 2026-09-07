---
description: ''
domains: []
hosts:
- dns:
    a: []
    aaaa: []
    cname: []
    note: Authoritative NOERROR with an empty answer section for A and AAAA — the zone exists and is delegated to AWS Route 53 (ns-219.awsdns-27.com, ns-815.awsdns-37.net, ns-1382.awsdns-44.org, ns-1863.awsdns-40.co.uk) but publishes no address record.
    resolves_to_address: false
  host: 4info.com
  https:
    cert_expires: null
    error: 'curl (6) Could not resolve host: 4info.com'
    hsts: null
    http_status: 0
    reachable: false
    tls_version: null
- dns:
    a: []
    aaaa: []
    cname: []
    resolves_to_address: false
  host: www.4info.com
  https:
    cert_expires: null
    error: 'curl (6) Could not resolve host: www.4info.com'
    hsts: null
    http_status: 0
    reachable: false
    tls_version: null
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: 4Info Domain Security
name_suffix: Domain Security
overview: Domain security posture for 4Info, probed live across 2 host(s) and 0 registrable domain(s). 2 host(s) serve HTTPS; 0 advertise HSTS.
provider_name: 4Info
provider_slug: 4info
slug: 4info-domain-security
source_filename: 4info-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: >-\n  DNS + TLS probes run directly against 4info.com and www.4info.com on 2026-09-05\n  (dig for A/AAAA/CNAME/MX/TXT/CAA/DNSKEY/DS/_dmarc, curl for HTTPS).\nname: 4Info\nslug: 4info\nsummary: >-\n  4info.com is a registered, actively delegated domain that is still used for EMAIL only.\n  It publishes no A or AAAA record on the apex or on www, so there is no web host to probe\n  for TLS, HSTS, or any HTTP surface at all. Mail is routed through Proofpoint and the\n  domain carries SPF and DMARC records, which is consistent with the domain being retained\n  by the acquirer (Cadent, January 2020) for mail continuity after the website was retired.\nregistrable_domain: 4info.com\nhosts:\n- host: 4info.com\n  dns:\n    a: []\n    aaaa: []\n    cname: []\n    resolves_to_address: false\n    note: >-\n      Authoritative NOERROR with an empty answer section for A and AAAA — the zone exists\n      and is delegated to AWS Route 53 (ns-219.awsdns-27.com,\
  \ ns-815.awsdns-37.net,\n      ns-1382.awsdns-44.org, ns-1863.awsdns-40.co.uk) but publishes no address record.\n  https:\n    reachable: false\n    http_status: 0\n    error: 'curl (6) Could not resolve host: 4info.com'\n    tls_version: null\n    cert_expires: null\n    hsts: null\n- host: www.4info.com\n  dns:\n    a: []\n    aaaa: []\n    cname: []\n    resolves_to_address: false\n  https:\n    reachable: false\n    http_status: 0\n    error: 'curl (6) Could not resolve host: www.4info.com'\n    tls_version: null\n    cert_expires: null\n    hsts: null\ndomain:\n  dnssec:\n    dnskey: false\n    ds: false\n    note: No DNSKEY at the zone apex and no DS at the parent — the zone is unsigned.\n  caa:\n    present: false\n    records: []\n    note: No CAA record — certificate issuance is not restricted to a named CA.\n  spf:\n    present: true\n    record: 'v=spf1 include:%{ir}.%{v}.%{d}.spf.has.pphosted.com -all'\n    policy: hard-fail\n    note: Proofpoint macro-expanded SPF include\
  \ with a -all hard fail.\n  dmarc:\n    present: true\n    record: 'v=DMARC1; p=none; fo=1; rua=mailto:dmarc_rua@emaildefense.proofpoint.com; ruf=mailto:dmarc_ruf@emaildefense.proofpoint.com;'\n    policy: none\n    note: >-\n      p=none is monitor-only — reports are collected by Proofpoint Email Defense but no\n      enforcement is requested on failing mail.\n  mx:\n    present: true\n    records:\n    - '10 mxa-003bca01.gslb.pphosted.com.'\n    - '10 mxb-003bca01.gslb.pphosted.com.'\n    provider: Proofpoint (pphosted.com)\nfindings:\n- The domain is alive for mail and dead for web; there is no HTTPS endpoint to assess.\n- DNSSEC is not enabled and no CAA record is published.\n- SPF and DMARC are both published; DMARC is at p=none (monitoring only).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/4info/refs/heads/main/security/4info-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Advertising
- AdTech
- Mobile Advertising
- Advanced TV
- Identity Resolution
- Audience Targeting
- Data
- Acquired
- Defunct
---
