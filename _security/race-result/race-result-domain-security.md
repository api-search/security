---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: raceresult.com
  spf: true
hosts:
- cert_expires: Aug 17 00:16:32 2026 GMT
  host: www.raceresult.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Race Result Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RACE RESULT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: RACE RESULT
provider_slug: race-result
slug: race-result-domain-security
source_filename: race-result-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.raceresult.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 00:16:32 2026 GMT\n  hsts: null\ndomains:\n- domain: raceresult.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/race-result/refs/heads/main/security/race-result-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Race Timing
- Decoder
- Sports
- Hardware
- Race Results
---
