---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: uu.net
  mx:
  - 15 omzsmtpe01.verizonbusiness.com
  - 15 omzsmtpe02.verizonbusiness.com
  - 15 omzsmtpe03.verizonbusiness.com
  - 15 omzsmtpe04.verizonbusiness.com
  - 30 fldsmtpe01.verizon.com
  - 30 fldsmtpe02.verizon.com
  nameservers:
  - auth00.ns.uu.net
  - auth60.ns.uu.net
  - auth200.ns.uu.net
  - auth210.ns.uu.net
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: uunet.com
  mx:
  - 10 mailstation.uu.net
  nameservers:
  - auth01.ns.uu.net
  - auth50.ns.uu.net
  - auth61.ns.uu.net
  - auth-ns1.verizonbusiness.com
  - auth-ns2.verizonbusiness.com
  spf: false
- dmarc: false
  dnssec: false
  domain: uunet.net
  nameservers:
  - auth03.ns.uu.net
  - auth50.ns.uu.net
  spf: false
hosts:
- dns: CNAME global.mci.com -> hostredirects.vzbtest.info -> 52.34.155.72
  host: www.uu.net
  hsts: false
  http_redirect: https://www.verizon.com/business/
  http_status: 301
  https: false
- dns: CNAME global.mci.com -> hostredirects.vzbtest.info -> 52.34.155.72
  host: www.uunet.com
  hsts: false
  http_redirect: https://www.verizon.com/business/
  http_status: 301
  https: false
- dns: no A record (NS + MX only)
  host: uu.net
  https: false
- dns: no A record (NS + MX only)
  host: uunet.com
  https: false
- dns: 192.48.96.9 (historic archive host A record still published)
  host: ftp.uu.net
  https: false
kind: domain-security
layout: security
method: probed
name: Uunet Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UUNET Technologies, probed live across 5 host(s) and 3 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: UUNET Technologies
provider_slug: uunet-technologies
slug: uunet-technologies-domain-security
source_filename: uunet-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of legacy UUNET domains (uu.net, uunet.com, uunet.net)\nnote: UUNET is a defunct brand (folded into Verizon Business). Its legacy DNS zones\n  remain operated by Verizon; web hosts serve only an HTTP 301 redirect to\n  https://www.verizon.com/business/ and do not serve HTTPS at all. Absence of\n  records below is real probed data, not a gap in probing.\nhosts:\n- host: www.uu.net\n  dns: CNAME global.mci.com -> hostredirects.vzbtest.info -> 52.34.155.72\n  https: false\n  http_status: 301\n  http_redirect: https://www.verizon.com/business/\n  hsts: false\n- host: www.uunet.com\n  dns: CNAME global.mci.com -> hostredirects.vzbtest.info -> 52.34.155.72\n  https: false\n  http_status: 301\n  http_redirect: https://www.verizon.com/business/\n  hsts: false\n- host: uu.net\n  dns: no A record (NS + MX only)\n  https: false\n- host: uunet.com\n  dns: no A record (NS + MX only)\n  https: false\n- host: ftp.uu.net\n\
  \  dns: 192.48.96.9 (historic archive host A record still published)\n  https: false\ndomains:\n- domain: uu.net\n  nameservers:\n  - auth00.ns.uu.net\n  - auth60.ns.uu.net\n  - auth200.ns.uu.net\n  - auth210.ns.uu.net\n  mx:\n  - 15 omzsmtpe01.verizonbusiness.com\n  - 15 omzsmtpe02.verizonbusiness.com\n  - 15 omzsmtpe03.verizonbusiness.com\n  - 15 omzsmtpe04.verizonbusiness.com\n  - 30 fldsmtpe01.verizon.com\n  - 30 fldsmtpe02.verizon.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: uunet.com\n  nameservers:\n  - auth01.ns.uu.net\n  - auth50.ns.uu.net\n  - auth61.ns.uu.net\n  - auth-ns1.verizonbusiness.com\n  - auth-ns2.verizonbusiness.com\n  mx:\n  - 10 mailstation.uu.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: uunet.net\n  nameservers:\n  - auth03.ns.uu.net\n  - auth50.ns.uu.net\n  dnssec: false\n  spf: false\n  dmarc: false\nwell_known:\n- path: /.well-known/security.txt\n  host: www.uu.net\n  status: unreachable (no HTTPS listener;\
  \ HTTP 301s to verizon.com)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uunet-technologies/refs/heads/main/security/uunet-technologies-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Internet Service Provider
- Networking
- Telecommunications
- Internet Backbone
- Defunct
---
