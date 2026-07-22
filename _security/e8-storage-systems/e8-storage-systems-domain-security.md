---
description: 'DNS and TLS posture probe of the historical E8 Storage Systems domain e8storage.com. The domain is retained but no longer serves web content: there is no A or AAAA record and no MX record, so the host does not resolve and cannot be reached over HTTPS. Authoritative nameservers are MarkMonitor and the DMARC aggregate/forensic reports are directed to dmarc.amazon.com, which is consistent with Amazon''s 2019 acquisition of the company and its retention of the domain as a defensive registration.'
domains:
- caa:
    present: false
    records: []
  dmarc:
    policy: reject
    present: true
    record: v=DMARC1; p=reject; rua=mailto:report@dmarc.amazon.com; ruf=mailto:report@dmarc.amazon.com
    reporting_org: amazon.com
  dnssec:
    dnskey: []
    ds: []
    enabled: false
  domain: e8storage.com
  hsts:
    note: not testable - no HTTPS endpoint
    present: false
  records:
    a: []
    aaaa: []
    mx: []
    ns:
    - ns1.markmonitor.com
    - ns2.markmonitor.com
    - ns3.markmonitor.com
    - ns4.markmonitor.com
    - ns5.markmonitor.com
    - ns6.markmonitor.com
    - ns7.markmonitor.com
    soa: ns1.markmonitor.com. hostmaster.markmonitor.com. 2023052501
  resolves: false
  spf:
    policy: hard-fail all senders (domain sends no mail)
    present: true
    record: v=spf1 -all
  tls:
    https_status: null
    note: not testable - no address record, connection could not be established
- domain: www.e8storage.com
  records:
    a: []
  resolves: false
hosts: []
kind: domain-security
layout: security
method: probed
name: E8 Storage Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for E8 Storage Systems, probed live across 0 host(s) and 2 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present.'
provider_name: E8 Storage Systems
provider_slug: e8-storage-systems
slug: e8-storage-systems-domain-security
source_filename: e8-storage-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: DNS/TLS probe of e8storage.com (dig + curl), 2026-07-20\nname: E8 Storage Systems Domain Security\ndescription: >-\n  DNS and TLS posture probe of the historical E8 Storage Systems domain\n  e8storage.com. The domain is retained but no longer serves web content: there\n  is no A or AAAA record and no MX record, so the host does not resolve and\n  cannot be reached over HTTPS. Authoritative nameservers are MarkMonitor and\n  the DMARC aggregate/forensic reports are directed to dmarc.amazon.com, which\n  is consistent with Amazon's 2019 acquisition of the company and its retention\n  of the domain as a defensive registration.\ndomains:\n  - domain: e8storage.com\n    resolves: false\n    records:\n      a: []\n      aaaa: []\n      mx: []\n      ns:\n        - ns1.markmonitor.com\n        - ns2.markmonitor.com\n        - ns3.markmonitor.com\n        - ns4.markmonitor.com\n        - ns5.markmonitor.com\n        - ns6.markmonitor.com\n\
  \        - ns7.markmonitor.com\n      soa: ns1.markmonitor.com. hostmaster.markmonitor.com. 2023052501\n    tls:\n      https_status: null\n      note: not testable - no address record, connection could not be established\n    hsts:\n      present: false\n      note: not testable - no HTTPS endpoint\n    dnssec:\n      enabled: false\n      dnskey: []\n      ds: []\n    caa:\n      present: false\n      records: []\n    spf:\n      present: true\n      record: v=spf1 -all\n      policy: hard-fail all senders (domain sends no mail)\n    dmarc:\n      present: true\n      record: 'v=DMARC1; p=reject; rua=mailto:report@dmarc.amazon.com; ruf=mailto:report@dmarc.amazon.com'\n      policy: reject\n      reporting_org: amazon.com\n  - domain: www.e8storage.com\n    resolves: false\n    records:\n      a: []\nfindings:\n  - severity: info\n    finding: >-\n      Domain is parked defensively, not operated. No A/AAAA/MX records and an\n      SPF hard-fail plus DMARC p=reject means the domain is\
  \ locked down against\n      spoofing while serving no traffic.\n  - severity: info\n    finding: >-\n      DMARC reporting addresses under dmarc.amazon.com indicate the domain is\n      administered by Amazon following the 2019 acquisition.\n  - severity: low\n    finding: DNSSEC is not enabled on the zone.\n  - severity: low\n    finding: No CAA records are published.\nprobes:\n  - target: https://e8storage.com/\n    status: null\n    result: DNS resolution failure (curl exit 6)\n  - target: https://www.e8storage.com/\n    status: null\n    result: DNS resolution failure (curl exit 6)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/e8-storage-systems/refs/heads/main/security/e8-storage-systems-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
- Big Data
- Storage
- NVMe
- Flash Storage
- Data Infrastructure
- Enterprise Storage
- Acquired
- Israel
---
