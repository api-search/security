---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: philzcoffee.com
  spf: true
hosts:
- cert_expires: Oct 10 14:03:25 2026 GMT
  host: www.philzcoffee.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Philz Coffee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Philz Coffee, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Philz Coffee
provider_slug: philz-coffee
slug: philz-coffee-domain-security
source_filename: philz-coffee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.philzcoffee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 14:03:25 2026 GMT\n  hsts: false\ndomains:\n- domain: philzcoffee.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/philz-coffee/refs/heads/main/security/philz-coffee-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Consumer
- Coffee
- Retail
- Beverage
- Food
---
