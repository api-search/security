---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: techstylefashiongroup.com
  note: Gandi-hosted parking + mail forwarding only.
  spf: true
  spf_record: v=spf1 include:_mailcust.gandi.net ?all
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: techstyle.com
  note: Live corporate mail domain behind Proofpoint (pphosted.com) with DMARC rua/ruf reporting to emaildefense.proofpoint.com; policy is p=none (monitor only). No CAA, no DNSSEC.
  spf: true
  spf_record: v=spf1 ... include:spf-00397e02.pphosted.com include:spf1.techstyle.com -all
- caa: []
  dmarc: false
  dnssec: false
  domain: techstyleos.com
  note: The TechStyle OS platform domain. Also parked at Gandi; TLS refused on 443, plain HTTP returns the same parking page.
  spf: true
  spf_record: v=spf1 include:_mailcust.gandi.net ?all
hosts:
- host: www.techstylefashiongroup.com
  https: false
  note: TLS handshake refused on port 443 (connection refused, Gandi webredir 217.70.184.50); HTTP 200 returns a 2,410-byte Gandi parking page for every path probed.
- host: www.techstyle.com
  https: true
  note: Answers HTTPS with a 301 to https://www.techstylefashiongroup.com/, which then fails to connect over TLS. No corporate content is served.
kind: domain-security
layout: security
method: probed
name: Techstyle Fashion Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Techstyle Fashion Group, probed live across 2 host(s) and 3 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Techstyle Fashion Group
provider_slug: techstyle-fashion-group
slug: techstyle-fashion-group-domain-security
source_filename: techstyle-fashion-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the TechStyle Fashion Group corporate domains\nnote: >-\n  The group has no HTTPS web presence. techstyle.com (the corporate domain named by the\n  company's own public record) 301s to www.techstylefashiongroup.com, which refuses TLS on\n  port 443 entirely and answers only on plain HTTP with a Gandi domain-parking page.\n  techstyle.com itself remains an active corporate MAIL domain — a large Proofpoint-fronted\n  SPF record and a DMARC record are published — so the company operates; it is the public\n  web surface that is gone. Brand hosts (fabletics.com, savagex.com, justfab.com,\n  shoedazzle.com) belong to the operating brands, which are profiled as separate providers.\nhosts:\n- host: www.techstylefashiongroup.com\n  https: false\n  note: >-\n    TLS handshake refused on port 443 (connection refused, Gandi webredir 217.70.184.50);\n    HTTP 200 returns a 2,410-byte Gandi parking page for every\
  \ path probed.\n- host: www.techstyle.com\n  https: true\n  note: >-\n    Answers HTTPS with a 301 to https://www.techstylefashiongroup.com/, which then fails to\n    connect over TLS. No corporate content is served.\ndomains:\n- domain: techstylefashiongroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 include:_mailcust.gandi.net ?all'\n  dmarc: false\n  note: Gandi-hosted parking + mail forwarding only.\n- domain: techstyle.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 ... include:spf-00397e02.pphosted.com include:spf1.techstyle.com -all'\n  dmarc: true\n  dmarc_policy: none\n  note: >-\n    Live corporate mail domain behind Proofpoint (pphosted.com) with DMARC rua/ruf reporting\n    to emaildefense.proofpoint.com; policy is p=none (monitor only). No CAA, no DNSSEC.\n- domain: techstyleos.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 include:_mailcust.gandi.net ?all'\n  dmarc: false\n  note: >-\n    The TechStyle OS platform\
  \ domain. Also parked at Gandi; TLS refused on 443, plain HTTP\n    returns the same parking page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/techstyle-fashion-group/refs/heads/main/security/techstyle-fashion-group-domain-security.yml
summary_line: DMARC
tags:
- Company
- Fashion
- Apparel
- Retail
- E-Commerce
- Direct to Consumer
- Subscription
- Holding Company
---
