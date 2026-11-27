---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pushpay.com
  spf: true
hosts:
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: pushpay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Church Community Builder (Pushpay) Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Church Community Builder (Pushpay), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Church Community Builder (Pushpay)
provider_slug: pushpay
slug: pushpay-domain-security
source_filename: pushpay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pushpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pushpay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/pushpay/security/pushpay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Church Giving
- Church Management Software
- Digital Giving
- Mobile App
- Donor Management
- Volunteer Management
- Live Streaming
---
