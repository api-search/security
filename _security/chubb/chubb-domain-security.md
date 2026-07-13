---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: chubb.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: chubbstudio.com
  spf: false
hosts:
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: www.chubb.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: chubbstudio.com
  https: false
kind: domain-security
layout: security
method: probed
name: Chubb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chubb, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Chubb
provider_slug: chubb
slug: chubb-domain-security
source_filename: chubb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chubb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: chubbstudio.com\n  https: false\ndomains:\n- domain: chubb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: chubbstudio.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chubb/refs/heads/main/security/chubb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Accident and Health
- Auto Insurance
- Claims
- Commercial Insurance
- Cyber Insurance
- Embedded Insurance
- Fortune 500
- Homeowners
- Insurance
- Life Insurance
- Marine
- Personal Insurance
- Property and Casualty
- Reinsurance
- Risk Management
- Travel Insurance
- Valuables
- Workers Compensation
---
