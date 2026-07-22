---
description: ''
domains:
- caa: []
  caa_evidence: dig CAA kuwo.cn returns only the apex CNAME igtmpg1.kuwo.cn; no CAA RRset is published
  dmarc: true
  dmarc_policy: none
  dmarc_record: v=DMARC1;p=none;rua=mailto:mailauth-reports@qq.com
  dnssec: false
  dnssec_evidence: no DS record at the .cn zone; no DNSKEY at kuwo.cn
  domain: kuwo.cn
  mail_note: SPF delegates to spf.mail.qq.com and DMARC aggregate reports route to mailauth-reports@qq.com, consistent with Tencent-operated mail.
  spf: true
  spf_record: v=spf1 include:spf.mail.qq.com ~all
hosts:
- host: kuwo.cn
  https: unknown
  note: DNS resolves (101.42.133.54, 101.42.130.11 plus IPv6) but TCP/443 connections time out from the probing network. Kuwo is a China-hosted consumer service and appears to be geo/firewall restricted, so TLS and HSTS posture could not be observed. This is a reachability failure, not evidence of missing HTTPS.
  reachable: false
kind: domain-security
layout: security
method: probed
name: Kuwo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kuwo Music, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kuwo Music
provider_slug: kuwo
slug: kuwo-domain-security
source_filename: kuwo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts (2026-07-19)\nnotes: >-\n  The apex kuwo.cn is served as a CNAME to igtmpg1.kuwo.cn (a non-standard apex\n  CNAME / CDN alias). Because the apex is a CNAME, every record-type query\n  returns that CNAME, which an automated probe can misread as a CAA record and\n  as DNSSEC material. Both were re-verified by hand: kuwo.cn publishes NO CAA\n  record and has NO DS record at the .cn zone, so DNSSEC is not enabled. SPF and\n  DMARC were confirmed as genuine TXT records.\nhosts:\n- host: kuwo.cn\n  https: unknown\n  reachable: false\n  note: >-\n    DNS resolves (101.42.133.54, 101.42.130.11 plus IPv6) but TCP/443 connections\n    time out from the probing network. Kuwo is a China-hosted consumer service\n    and appears to be geo/firewall restricted, so TLS and HSTS posture could not\n    be observed. This is a reachability failure, not evidence of missing HTTPS.\ndomains:\n- domain: kuwo.cn\n\
  \  dnssec: false\n  dnssec_evidence: no DS record at the .cn zone; no DNSKEY at kuwo.cn\n  caa: []\n  caa_evidence: >-\n    dig CAA kuwo.cn returns only the apex CNAME igtmpg1.kuwo.cn; no CAA RRset is\n    published\n  spf: true\n  spf_record: v=spf1 include:spf.mail.qq.com ~all\n  dmarc: true\n  dmarc_policy: none\n  dmarc_record: v=DMARC1;p=none;rua=mailto:mailauth-reports@qq.com\n  mail_note: >-\n    SPF delegates to spf.mail.qq.com and DMARC aggregate reports route to\n    mailauth-reports@qq.com, consistent with Tencent-operated mail.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kuwo/refs/heads/main/security/kuwo-domain-security.yml
summary_line: DMARC
tags:
- Company
- Music
- Streaming
- Media
- Entertainment
- Audio
- Consumer
- China
---
