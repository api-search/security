---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aidata.broker
  spf: false
hosts:
- cert_expires: Jan  9 09:30:55 2027 GMT
  host: aidata.broker
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aidata Broker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AIData.Broker open data API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: AIData.Broker open data API
provider_slug: aidata-broker
slug: aidata-broker-domain-security
source_filename: aidata-broker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aidata.broker\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 09:30:55 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aidata.broker\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aidata-broker/refs/heads/main/security/aidata-broker-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Marketplace
- AI Training
- Pricing
- Buyers
---
