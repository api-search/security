---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aeronext.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: aeronext.co.jp
  spf: true
  spf_record: v=spf1 +a:sv8009.xserver.jp +a:aeronext.co.jp +mx include:spf.sender.xserver.jp ~all
- caa: []
  dmarc: false
  dnssec: false
  domain: skyhub.jp
  spf: true
  spf_record: v=spf1 +a:sv8009.xserver.jp +a:skyhub.jp +mx ip4:153.121.77.125 include:spf.sender.xserver.jp include:_spf.google.com ~all
- caa: []
  dmarc: true
  dmarc_record: v=DMARC1; p=none;
  dnssec: false
  domain: nextdelivery.co.jp
  spf: false
hosts:
- cert_expires: Nov  1 22:14:20 2026 GMT
  host: aeronext.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 02:29:37 2026 GMT
  host: aeronext.co.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 23:09:03 2026 GMT
  host: nextdelivery.co.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 04:09:10 2026 GMT
  host: skyhub.jp
  hsts: false
  https: true
  note: 'SkyHub marketing site, operated by NEXT DELIVERY Inc. (footer: (c) 2023 NEXT DELIVERY Inc.)'
  tls_version: TLSv1.3
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: tms.skyhub.jp
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: SkyHub TMS application (React SPA). The only Aeronext-group host that sets HSTS.
  tls_version: TLSv1.3
hosts_probed: 5
kind: domain-security
layout: security
method: probed
name: Aeronext Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aeronext, probed live across 5 host(s) and 4 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Aeronext
provider_slug: aeronext
slug: aeronext-domain-security
source_filename: aeronext-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of every host Aeronext Inc. and its subsidiary NEXT DELIVERY Inc. operate (aeronext.com,\n  aeronext.co.jp, nextdelivery.co.jp, skyhub.jp, tms.skyhub.jp)\nhosts:\n- host: aeronext.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 22:14:20 2026 GMT\n  hsts: false\n- host: aeronext.co.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 02:29:37 2026 GMT\n  hsts: false\n- host: nextdelivery.co.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 23:09:03 2026 GMT\n  hsts: false\n- host: skyhub.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 04:09:10 2026 GMT\n  hsts: false\n  note: 'SkyHub marketing site, operated by NEXT DELIVERY Inc. (footer: (c) 2023 NEXT DELIVERY Inc.)'\n- host: tms.skyhub.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: SkyHub TMS application\
  \ (React SPA). The only Aeronext-group host that sets HSTS.\ndomains:\n- domain: aeronext.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: aeronext.co.jp\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 +a:sv8009.xserver.jp +a:aeronext.co.jp +mx include:spf.sender.xserver.jp ~all\n  dmarc: false\n- domain: skyhub.jp\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 +a:sv8009.xserver.jp +a:skyhub.jp +mx ip4:153.121.77.125 include:spf.sender.xserver.jp include:_spf.google.com\n    ~all\n  dmarc: false\n- domain: nextdelivery.co.jp\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_record: v=DMARC1; p=none;\nfindings:\n- All five hosts serve HTTPS over TLS 1.3 with valid certificates.\n- HSTS is set on tms.skyhub.jp only (max-age=31536000); the four content sites set no Strict-Transport-Security\n  header.\n- No domain in the group publishes DNSSEC or CAA records.\n- SPF is published for aeronext.com, aeronext.co.jp and skyhub.jp\
  \ (all Xserver-hosted mail); nextdelivery.co.jp\n  has no SPF.\n- DMARC exists only on nextdelivery.co.jp, at p=none (monitor-only, no enforcement).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aeronext/refs/heads/main/security/aeronext-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Drones
- UAV
- Logistics
- Last Mile Delivery
- Transportation
- Robotics
- Aerospace
- Supply Chain
- Japan
---
