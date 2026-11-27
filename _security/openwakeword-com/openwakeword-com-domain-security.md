---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: openwakeword.com
  spf: true
hosts:
- cert_expires: Jan 30 04:13:10 2027 GMT
  host: openwakeword.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OpenWakeWord Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenWakeWord, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: OpenWakeWord
provider_slug: openwakeword-com
slug: openwakeword-com-domain-security
source_filename: openwakeword-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openwakeword.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 04:13:10 2027 GMT\n  hsts: false\ndomains:\n- domain: openwakeword.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/openwakeword-com/security/openwakeword-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Open Source
- Voice AI
- Wake Word
- Home Automation
---
