---
description: Transport and DNS security posture probed for the Phone.com public API host and marketing host. Absence of a record is valid, expected data.
domains: []
hosts:
- host: api.phone.com
  hsts: false
  http_version: HTTP/2
  note: Returns HTTP 401 without a token (all endpoints require OAuth). TLS negotiated successfully.
  tls: true
- host: www.phone.com
  hsts: false
  http_version: HTTP/2
  tls: true
kind: domain-security
layout: security
method: probed
name: Phone Com Domain Security
name_suffix: Domain Security
overview: Domain security posture for Phone Com, probed live across 2 host(s) and 0 registrable domain(s).
provider_name: Phone Com
provider_slug: phone-com
slug: phone-com-domain-security
source_filename: phone-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: manual probe (curl/dig)\ntype: DomainSecurity\ndescription: >-\n  Transport and DNS security posture probed for the Phone.com public API host\n  and marketing host. Absence of a record is valid, expected data.\nhosts:\n- host: api.phone.com\n  tls: true\n  http_version: HTTP/2\n  hsts: false\n  note: Returns HTTP 401 without a token (all endpoints require OAuth). TLS negotiated successfully.\n- host: www.phone.com\n  tls: true\n  http_version: HTTP/2\n  hsts: false\ndns:\n  domain: phone.com\n  dnssec: false\n  caa: false\n  spf: true\n  spf_record: \"v=spf1 ip4:72.1.46.0/23 include:_spf.google.com include:spf.mandrillapp.com include:stspg-customer.com include:spf.smtp2go.com include:_spf.salesforce.com include:amazonses.com include:spf.protection.outlook.com ~all\"\n  dmarc: true\n  dmarc_policy: none\n  dmarc_record: \"v=DMARC1; p=none; sp=none; rua=mailto:dmarc@phone.com\"\nfindings:\n- SPF and DMARC are published (DMARC at\
  \ monitor-only p=none).\n- No DNSSEC (no DS record) and no CAA record at the apex.\n- HSTS not observed on either the API or marketing host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phone-com/refs/heads/main/security/phone-com-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- VoIP
- Telephony
- Business Phone
- SMS
- Video Conferencing
- Communications
---
