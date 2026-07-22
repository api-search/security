---
description: ''
domains:
- caa: []
  caa_note: No CAA record published. The automated probe recorded wfgqda.r23.35.cn., which is the CNAME target in the resolution chain, not a CAA record.
  dmarc: true
  dmarc_policy: quarantine
  dmarc_record: v=DMARC1; p=quarantine; fo=1; ruf=mailto:dmarc@qiye.163.com; rua=mailto:dmarc_report@qiye.163.com
  dnssec: false
  domain: letel.com.cn
  spf: true
  spf_record: v=spf1 include:spf.163.com -all
hosts:
- cert_issuer: Sectigo Public Server Authentication CA DV R36
  cert_not_after: '2027-01-18'
  host: letel.com.cn
  hsts: unknown
  hsts_note: WAF returns 403 to header probes
  https: true
  tls_verify: ok
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Letel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Letel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Letel
provider_slug: letel
slug: letel-domain-security
source_filename: letel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts\nnotes: >-\n  letel.com.cn sits behind a JavaScript bot-check WAF that returns 403 to HEAD\n  and non-browser requests, so the automated HTTP probe under-reported HTTPS.\n  TLS was confirmed directly with an openssl s_client handshake. HSTS could not\n  be observed because the WAF rejects the request before response headers are\n  emitted; recorded as unknown rather than false.\nhosts:\n- host: letel.com.cn\n  https: true\n  tls_version: TLSv1.3\n  tls_verify: ok\n  cert_issuer: Sectigo Public Server Authentication CA DV R36\n  cert_not_after: '2027-01-18'\n  hsts: unknown\n  hsts_note: WAF returns 403 to header probes\ndomains:\n- domain: letel.com.cn\n  dnssec: false\n  caa: []\n  caa_note: >-\n    No CAA record published. The automated probe recorded wfgqda.r23.35.cn.,\n    which is the CNAME target in the resolution chain, not a CAA record.\n  spf: true\n  spf_record: v=spf1 include:spf.163.com\
  \ -all\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_record: v=DMARC1; p=quarantine; fo=1; ruf=mailto:dmarc@qiye.163.com; rua=mailto:dmarc_report@qiye.163.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/letel/refs/heads/main/security/letel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Centers
- Networking
- Telecommunications
- Hardware
- Manufacturing
- Infrastructure
- China
---
