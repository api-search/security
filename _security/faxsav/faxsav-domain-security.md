---
description: ''
domains:
- a_records:
  - 150.105.185.81
  - 150.105.219.25
  caa: []
  created: '1995-06-29'
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: faxsav.com
  mx:
  - ev3-bigip-lt.lt.easylink.com
  - ev3-bigip-al.al.easylink.com
  nameservers:
  - ns1.opntxtdns.com
  - ns2.opntxtdns.com
  - ns4.opntxtdns.com
  - ns5.opntxtdns.com
  registered: true
  registrar: SafeNames Ltd.
  registry_expiry: '2026-12-02'
  spf: false
hosts:
- host: faxsav.com
  http_status: null
  https: false
  probe_result: connection timed out (ports 80 and 443 filtered/closed)
- host: www.faxsav.com
  http_status: null
  https: false
  probe_result: connection timed out
kind: domain-security
layout: security
method: probed
name: Faxsav Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FaxSav, probed live across 2 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: FaxSav
provider_slug: faxsav
slug: faxsav-domain-security
source_filename: faxsav-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of faxsav.com (2026-07-20)\nnotes: >-\n  FaxSav is a defunct company (merged into Mail.com in 2000; lineage now inside\n  OpenText). faxsav.com is still registered and DNS-delegated to OpenText\n  nameservers (opntxtdns.com) with MX pointing at easylink.com, but no web\n  server answers on port 80 or 443 — connections time out. Absence of records\n  below is measured, not assumed.\nhosts:\n- host: faxsav.com\n  https: false\n  http_status: null\n  probe_result: connection timed out (ports 80 and 443 filtered/closed)\n- host: www.faxsav.com\n  https: false\n  http_status: null\n  probe_result: connection timed out\ndomains:\n- domain: faxsav.com\n  registered: true\n  registrar: SafeNames Ltd.\n  created: '1995-06-29'\n  registry_expiry: '2026-12-02'\n  nameservers:\n  - ns1.opntxtdns.com\n  - ns2.opntxtdns.com\n  - ns4.opntxtdns.com\n  - ns5.opntxtdns.com\n  a_records:\n  - 150.105.185.81\n  - 150.105.219.25\n\
  \  mx:\n  - ev3-bigip-lt.lt.easylink.com\n  - ev3-bigip-al.al.easylink.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  dmarc_policy: null\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/faxsav/refs/heads/main/security/faxsav-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Fax
- Internet Fax
- Messaging
- Communications
- Document Delivery
- Telecommunications
- Defunct
- Historical
---
