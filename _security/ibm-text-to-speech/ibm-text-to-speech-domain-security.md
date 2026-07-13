---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ibm.com
  spf: true
hosts:
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: cloud.ibm.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ibm Text To Speech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IBM Text to Speech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: IBM Text to Speech
provider_slug: ibm-text-to-speech
slug: ibm-text-to-speech-domain-security
source_filename: ibm-text-to-speech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloud.ibm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: ibm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ibm-text-to-speech/refs/heads/main/security/ibm-text-to-speech-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Development
- Public APIs
---
