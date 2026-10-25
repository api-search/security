---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: perseusmining.com
  spf: true
hosts:
- cert_expires: Dec  9 06:28:55 2026 GMT
  host: perseusmining.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Perseus Mining Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Perseus Mining, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Perseus Mining
provider_slug: perseus-mining
slug: perseus-mining-domain-security
source_filename: perseus-mining-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: perseusmining.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 06:28:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: perseusmining.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perseus-mining/refs/heads/main/security/perseus-mining-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Mining
- Gold
- Natural Resources
- Australia
- Africa
- ASX Listed
---
