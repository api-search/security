---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: iris-amoi.com
  spf: true
  spf_record: v=spf1 ip4:183.251.83.28 ip4:218.5.71.34 ip4:183.251.83.30 include:spf.mail.qq.com ~all
hosts:
- cert_expires: Nov 12 12:45:05 2026 GMT
  host: www.iris-amoi.com
  hsts: null
  http_plain_served: true
  https: true
  note: Plain http:// is served without redirect to https://; no Strict-Transport-Security header.
  server: Microsoft-IIS/8.5
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aires1Ff5 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aires (IRIS Xiamen Science), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Aires (IRIS Xiamen Science)
provider_slug: aires1ff5
slug: aires1ff5-domain-security
source_filename: aires1ff5-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts (probe-domain-security.py, DNS fields re-verified by hand with dig)\nnote: >-\n  iris-amoi.com is a CNAME at the apex (iris-amoi.com -> iris-amoi.com.qzkey.com -> yd3.by-44kqk.ty3w.net),\n  so `dig +short <type>` returns the CNAME chain for every record type and probe-domain-security.py\n  initially recorded dnssec: true and two CAA \"records\" that were in fact CNAME targets. Re-verified:\n  no DS record at the parent, no DNSKEY, no CAA, no _dmarc TXT. Values below are the corrected ones.\nhosts:\n- host: www.iris-amoi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 12 12:45:05 2026 GMT\n  hsts: null\n  server: Microsoft-IIS/8.5\n  http_plain_served: true\n  note: Plain http:// is served without redirect to https://; no Strict-Transport-Security header.\ndomains:\n- domain: iris-amoi.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 ip4:183.251.83.28\
  \ ip4:218.5.71.34 ip4:183.251.83.30 include:spf.mail.qq.com ~all'\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aires1ff5/refs/heads/main/security/aires1ff5-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Contact Lenses
- Manufacturing
- Medical Devices
- Vision Care
- Optics
- Consumer Goods
- ODM
- China
---
