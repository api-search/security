---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: woohoo.in
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: qwikcilver.in
  spf: true
hosts:
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: www.woohoo.in
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 15:01:01 2026 GMT
  host: developer.qwikcilver.in
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: api.woohoo.in
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qwikcilver Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for QwikCilver, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: QwikCilver
provider_slug: qwikcilver
slug: qwikcilver-domain-security
source_filename: qwikcilver-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.woohoo.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.qwikcilver.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 15:01:01 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: api.woohoo.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: woohoo.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: qwikcilver.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qwikcilver/refs/heads/main/security/qwikcilver-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Gift Cards
- Prepaid
- Payments
- Fintech
- Rewards
- Corporate Gifting
- India
---
