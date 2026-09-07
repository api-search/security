---
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_record: null
  dnssec: false
  domain: vipkid.com
  spf: true
  spf_record: '"v=spf1 +include:_netblocks.m.feishu.cn -all"'
- caa: []
  dmarc: true
  dmarc_record: '"v=DMARC1; p=quarantine; fo=1; ruf=mailto:dmarc@qiye.163.com; rua=mailto:dmarc_report@qiye.163.com"'
  dnssec: false
  domain: vipkid.com.cn
  spf: true
  spf_record: '"v=spf1 include:spf.qiye.163.com -all"'
- caa: []
  dmarc: true
  dmarc_record: '"v=DMARC1; p=none; rua=dmarc-reports@vipteacher.com"'
  dnssec: false
  domain: vipteacher.com
  spf: true
  spf_record: '"v=spf1 include:mailgun.org ~all"'
hosts:
- cert_expires: Nov 26 05:53:40 2026 GMT
  host: www.vipkid.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: vipkid.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: m.vipkid.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: www.vipkid.com.cn
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: www.vipteacher.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: teach.vipteacher.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 6
kind: domain-security
layout: security
method: probed
name: Vipkid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VIPKid, probed live across 6 host(s) and 3 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: VIPKid
provider_slug: vipkid
slug: vipkid-domain-security
source_filename: vipkid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of every VIPKid / VIPTeacher host in apis.yml and named by the site's\n  own markup\nprovider: VIPKid\nsummary: 'All six VIPKid / VIPTeacher hosts serve HTTPS with a valid certificate — the two Nuxt\n  marketing hosts negotiate TLS 1.3, the four behind the Akamai/Tengine edge negotiate TLS 1.2 — but\n  the wider domain posture is thin: not one host sets HSTS, none of the three registrable domains is\n  DNSSEC-signed, none publishes a CAA record, and vipkid.com has SPF but no DMARC record at all.\n  vipkid.com.cn (p=quarantine) and vipteacher.com (p=none) do publish DMARC. Absence of a record here\n  is an observed fact, not a failed lookup.'\nhosts:\n- host: www.vipkid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 05:53:40 2026 GMT\n  hsts: false\n- host: vipkid.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: false\n- host: m.vipkid.com\n\
  \  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: false\n- host: www.vipkid.com.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: false\n- host: www.vipteacher.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: false\n- host: teach.vipteacher.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: vipkid.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: '\"v=spf1 +include:_netblocks.m.feishu.cn -all\"'\n  dmarc: false\n  dmarc_record: null\n- domain: vipkid.com.cn\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: '\"v=spf1 include:spf.qiye.163.com -all\"'\n  dmarc: true\n  dmarc_record: '\"v=DMARC1; p=quarantine; fo=1; ruf=mailto:dmarc@qiye.163.com; rua=mailto:dmarc_report@qiye.163.com\"'\n- domain: vipteacher.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: '\"v=spf1 include:mailgun.org\
  \ ~all\"'\n  dmarc: true\n  dmarc_record: '\"v=DMARC1; p=none; rua=dmarc-reports@vipteacher.com\"'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vipkid/refs/heads/main/security/vipkid-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Education
- EdTech
- Online Learning
- Language Learning
- English Language Teaching
- Tutoring
- K-12
- Consumer
- China
---
