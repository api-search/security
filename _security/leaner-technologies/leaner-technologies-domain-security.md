---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: leaner.co.jp
  spf: true
- caa: []
  dmarc: true
  dmarc_delegated: hosteddmarc.dmarc-dns.com (PowerDMARC)
  dmarc_policy: none
  dnssec: false
  domain: leaner.jp
  spf: true
  spf_record: v=spf1 include:spf.mta.hdems.com include:_spf.google.com ~all
hosts:
- cert_expires: Oct  1 10:19:30 2026 GMT
  host: leaner.co.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 07:35:46 2026 GMT
  host: leaner.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Leaner Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Leaner Technologies, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Leaner Technologies
provider_slug: leaner-technologies
slug: leaner-technologies-domain-security
source_filename: leaner-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts\nhosts:\n- host: leaner.co.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 10:19:30 2026 GMT\n  hsts: false\n- host: leaner.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 07:35:46 2026 GMT\n  hsts: false\ndomains:\n- domain: leaner.co.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: leaner.jp\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:spf.mta.hdems.com include:_spf.google.com ~all\n  dmarc: true\n  dmarc_policy: none\n  dmarc_delegated: hosteddmarc.dmarc-dns.com (PowerDMARC)\nnotes:\n- Neither corporate (leaner.co.jp) nor product (leaner.jp) host sets HSTS.\n- No CAA records and no DNSSEC on either registrable domain.\n- DMARC is published on both domains but at p=none (monitor only, not enforcing).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leaner-technologies/refs/heads/main/security/leaner-technologies-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cloud
- Procurement
- Purchasing
- Spend Management
- Sourcing
- Supplier Relationship Management
- Enterprise SaaS
- Japan
- Indirect Spend
---
