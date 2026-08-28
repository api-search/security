---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: qomplx.com
  spf: false
hosts:
- cert_expires: Sep 16 07:42:38 2026 GMT
  host: www.qomplx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qomplx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qomplx, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Qomplx
provider_slug: qomplx
slug: qomplx-domain-security
source_filename: qomplx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.qomplx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 07:42:38 2026 GMT\n  hsts: false\ndomains:\n- domain: qomplx.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\nnotes:\n  verified_independently: >-\n    Re-checked with dig on 2026-08-26. qomplx.com carries Google Workspace MX records\n    (aspmx.l.google.com et al.) and two TXT verification records (Atlassian, Box), but publishes\n    NO SPF record, NO _dmarc TXT record, NO CAA record and no DNSSEC. www.qomplx.com serves no\n    Strict-Transport-Security header. All five absences are the observed state, not a probe\n    failure.\n  significance: >-\n    QOMPLX sells identity-threat detection, managed detection and response, and attack-surface\n    monitoring. A mail domain with live MX and no SPF or DMARC is spoofable, and it is the same\n    class of exposure the company's\
  \ own attack-surface product is sold to find.\n  vulnerability_disclosure:\n    published: advertised-but-unreachable\n    security_txt:\n      url: https://www.qomplx.com/.well-known/security.txt\n      status: 404\n    pages:\n    - url: https://www.qomplx.com/vulnerability-disclosure-policy/\n      status: 301\n      result: self-redirect loop; unreadable\n    - url: https://www.qomplx.com/bug-bounties/\n      status: 301\n      result: self-redirect loop; unreadable\n    note: >-\n      QOMPLX lists both a vulnerability-disclosure policy and a bug-bounties page in its own\n      sitemap, so the program is intended to be public, but neither document can be retrieved. No\n      Security, SecurityTxt or VulnerabilityDisclosure pointer is emitted in apis.yml — pointing\n      at an unreachable page would assert a program a researcher cannot actually read.\n  trust_center:\n    published: false\n    probes:\n    - url: https://trust.qomplx.com/\n      status: 0\n      result: DNS does not\
  \ resolve\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qomplx/refs/heads/main/security/qomplx-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Cybersecurity
- Identity Threat Detection
- Managed Detection and Response
- Attack Surface Management
- Time Series
- Analytics
- Risk Management
- Insurance
- Data Platform
---
