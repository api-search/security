---
description: ''
domains:
- caa: false
  dmarc: false
  dnssec: false
  domain: 5lmeet.com
  mx:
  - mxbiz1.qq.com
  - mxbiz2.qq.com
  mx_note: Tencent Exmail — the domain is still in use for corporate email
  registrar: Alibaba Cloud Computing (Beijing) Co., Ltd.
  registry_expiry: '2027-04-12'
  spf: false
hosts:
- dns_a:
  - 8.140.56.113
  - 39.98.123.89
  - 60.205.152.91
  host: www.5lmeet.com
  hsts: false
  http: 200
  http_body: unconfigured "IIS Windows Server" default page (703 bytes)
  https: false
  https_note: no listener on port 443 on any of the three A records — connection refused on 39.98.123.89, timeout on 8.140.56.113 and 60.205.152.91
  tls: null
- dns_a:
  - 101.201.52.28
  host: api.5lmeet.com
  http: null
  https: false
  https_note: TCP connect fails on both port 80 and port 443 (filtered / no listener)
- dns_a:
  - 101.201.52.28
  host: m.5lmeet.com
  http: null
  https: false
  https_note: TCP connect fails on both port 80 and port 443 (filtered / no listener)
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: 5Lmeet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 5Lmeet, probed live across 3 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: 5Lmeet
provider_slug: 5lmeet
slug: 5lmeet-domain-security
source_filename: 5lmeet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of 5lmeet.com, 2026-09-05\nnote: >-\n  probe-domain-security.py returned \"unreachable\" and declined to write, because the domain has\n  no reachable HTTPS endpoint and carries none of the DNS security records it looks for. That\n  result is itself the measurement, so it is recorded here by hand from the same probes rather\n  than left as a silent gap. 5lmeet.com is a live, renewed registration (Alibaba Cloud Computing\n  (Beijing), expires 2027-04-12) with working Tencent Exmail MX records, so the domain is still\n  held and still used for corporate email — but it serves no TLS, publishes no SPF, DMARC, CAA\n  or DNSSEC, and its web root returns the stock unconfigured IIS welcome page.\nhosts:\n  - host: www.5lmeet.com\n    dns_a:\n      - 8.140.56.113\n      - 39.98.123.89\n      - 60.205.152.91\n    http: 200\n    http_body: unconfigured \"IIS Windows Server\" default page (703 bytes)\n    https:\
  \ false\n    https_note: >-\n      no listener on port 443 on any of the three A records — connection refused on\n      39.98.123.89, timeout on 8.140.56.113 and 60.205.152.91\n    tls: null\n    hsts: false\n  - host: api.5lmeet.com\n    dns_a:\n      - 101.201.52.28\n    http: null\n    https: false\n    https_note: TCP connect fails on both port 80 and port 443 (filtered / no listener)\n  - host: m.5lmeet.com\n    dns_a:\n      - 101.201.52.28\n    http: null\n    https: false\n    https_note: TCP connect fails on both port 80 and port 443 (filtered / no listener)\ndomains:\n  - domain: 5lmeet.com\n    registrar: Alibaba Cloud Computing (Beijing) Co., Ltd.\n    registry_expiry: '2027-04-12'\n    dnssec: false\n    caa: false\n    spf: false\n    dmarc: false\n    mx:\n      - mxbiz1.qq.com\n      - mxbiz2.qq.com\n    mx_note: Tencent Exmail — the domain is still in use for corporate email\nfindings:\n  - no HTTPS is offered on any host under the domain; the site is plain HTTP only\n\
  \  - no HSTS, no CAA, no DNSSEC\n  - no SPF and no DMARC record, despite active Tencent Exmail MX records\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/5lmeet/refs/heads/main/security/5lmeet-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Real Estate
- Coworking
- Co-Living
- Workspace
- Property Technology
- Hospitality
- Urban Development
- China
---
