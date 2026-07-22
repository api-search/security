---
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: likeplum.com
  spf: true
  spf_record: v=spf1 include:spf.protection.outlook.com -all
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: studypool.com
  spf: true
hosts:
- cert_expires: Jan 20 14:22:03 2027 GMT
  host: likeplum.com
  hsts: false
  https: true
  redirects_to: https://www.studypool.com/
  tls_version: TLSv1.3
- cert_expires: Oct  9 23:40:36 2026 GMT
  host: studypool.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Likeplum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Likeplum, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Likeplum
provider_slug: likeplum
slug: likeplum-domain-security
source_filename: likeplum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts (likeplum.com + successor studypool.com)\nnotes: >-\n  likeplum.com still resolves and serves TLS, but 301-redirects all traffic to\n  www.studypool.com, the surviving property of the former Createpool network.\n  Both hosts are probed here.\nhosts:\n- host: likeplum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 14:22:03 2027 GMT\n  hsts: false\n  redirects_to: https://www.studypool.com/\n- host: studypool.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:40:36 2026 GMT\n  hsts: false\ndomains:\n- domain: likeplum.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:spf.protection.outlook.com -all\n  dmarc: false\n  dmarc_policy: null\n- domain: studypool.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/likeplum/refs/heads/main/security/likeplum-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Marketplace
- Expert Network
- Question And Answer
- Freelance
- Gig Economy
- Education
- Rebranded
---
