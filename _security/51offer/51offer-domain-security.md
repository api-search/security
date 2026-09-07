---
api_specs:
- filename: 51offer-horizon-site-openapi.yml
  format: yaml
  label: 51offer Horizon Site API
  slug: 51offer-horizon-site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/51offer/refs/heads/main/openapi/51offer-horizon-site-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_note: _dmarc.51offer.com returns NXDOMAIN
  dnssec: false
  domain: 51offer.com
  mx:
  - 51offer-com.corpsmtp.net
  - 51offer-com.corpsmtp.cn
  - cnc.biz-email.net
  - mail.biz-email.net
  nameservers:
  - f1g1ns1.dnspod.net
  note: SPF is published with a hard fail (-all). No DNSSEC, no CAA and no DMARC record exists.
  spf: true
  spf_record: v=spf1 ip4:47.100.215.175 include:_s.corp-email.com -all
hosts:
- certificate_issuer: C=CN, O=Beijing Xinchacha Credit Management Co., Ltd., CN=Xcc Trust DV SSL CA
  certificate_not_after: '2026-10-21'
  certificate_not_before: '2025-10-21'
  certificate_subject: CN=*.51offer.com
  certificate_verify: ok
  cipher: ECDHE-RSA-AES256-GCM-SHA384
  host: www.51offer.com
  hsts: false
  https: true
  note: No Strict-Transport-Security header. TLS 1.3 not negotiated; the host settles on TLS 1.2.
  tls_version: TLSv1.2
- host: m.51offer.com
  hsts: false
  https: true
  note: Serves the same Swagger 1.2 documents at /api-docs.
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: 51Offer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 51offer, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: 51offer
provider_slug: 51offer
slug: 51offer-domain-security
source_filename: 51offer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live TLS/HTTP probes of www.51offer.com and m.51offer.com plus DNS lookups of 51offer.com against 8.8.8.8,\n  2026-09-05. Re-probed by hand after probe-domain-security.py recorded https:false for www.51offer.com on a transient\n  connection failure - the host does serve HTTPS.\nhosts:\n- host: www.51offer.com\n  https: true\n  tls_version: TLSv1.2\n  cipher: ECDHE-RSA-AES256-GCM-SHA384\n  certificate_subject: CN=*.51offer.com\n  certificate_issuer: C=CN, O=Beijing Xinchacha Credit Management Co., Ltd., CN=Xcc Trust DV SSL CA\n  certificate_not_before: '2025-10-21'\n  certificate_not_after: '2026-10-21'\n  certificate_verify: ok\n  hsts: false\n  note: No Strict-Transport-Security header. TLS 1.3 not negotiated; the host settles on TLS 1.2.\n- host: m.51offer.com\n  https: true\n  hsts: false\n  note: Serves the same Swagger 1.2 documents at /api-docs.\ndomains:\n- domain: 51offer.com\n  dnssec: false\n  caa: []\n  spf: true\n\
  \  spf_record: v=spf1 ip4:47.100.215.175 include:_s.corp-email.com -all\n  dmarc: false\n  dmarc_note: _dmarc.51offer.com returns NXDOMAIN\n  mx:\n  - 51offer-com.corpsmtp.net\n  - 51offer-com.corpsmtp.cn\n  - cnc.biz-email.net\n  - mail.biz-email.net\n  nameservers:\n  - f1g1ns1.dnspod.net\n  note: SPF is published with a hard fail (-all). No DNSSEC, no CAA and no DMARC record exists.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/51offer/refs/heads/main/security/51offer-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Education
- Study Abroad
- Higher Education
- University Applications
- Students
- Language Training
- E-Commerce
- China
- Consulting
---
