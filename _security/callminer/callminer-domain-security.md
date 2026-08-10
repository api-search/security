---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: callminer.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: callminer.net
  spf: true
hosts:
- cert_expires: Mar 12 23:59:59 2027 GMT
  host: callminer.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 23:59:59 2026 GMT
  host: api.callminer.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Callminer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CallMiner, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CallMiner
provider_slug: callminer
slug: callminer-domain-security
source_filename: callminer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: callminer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 12 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: api.callminer.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: callminer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: callminer.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/callminer/refs/heads/main/security/callminer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Conversation Intelligence
- Speech Analytics
- Contact Center
- Customer Experience
- Artificial Intelligence
- Analytics
- Transcription
- Quality Management
- Compliance
---
