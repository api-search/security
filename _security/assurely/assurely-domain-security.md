---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: assurely.com
  spf: true
hosts:
- cert_expires: Oct 13 18:24:45 2026 GMT
  host: www.assurely.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Assurely Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Assurely, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Assurely
provider_slug: assurely
slug: assurely-domain-security
source_filename: assurely-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.assurely.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 18:24:45 2026 GMT\n  hsts: null\ndomains:\n- domain: assurely.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/assurely/refs/heads/main/security/assurely-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Insurance
- United States
- Insurtech
- Embedded Insurance
- Managing General Agent
- Property and Casualty
- Directors and Officers
- Brokers
- Crowdfunding
---
