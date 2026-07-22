---
description: ''
domains:
- caa:
  - 0 issuewild "globalsign.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bharatmatrimony.in
  spf: true
hosts:
- cert_expires: Apr 10 09:06:35 2027 GMT
  host: www.bharatmatrimony.in
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bharat Matrimony Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bharat Matrimony, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bharat Matrimony
provider_slug: bharat-matrimony
slug: bharat-matrimony-domain-security
source_filename: bharat-matrimony-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bharatmatrimony.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 10 09:06:35 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bharatmatrimony.in\n  dnssec: false\n  caa:\n  - 0 issuewild \"globalsign.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bharat-matrimony/refs/heads/main/security/bharat-matrimony-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Matrimony
- Matchmaking
- Dating
- Relationships
- India
---
