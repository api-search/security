---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fieldtranscript.com
  spf: true
hosts:
- cert_expires: Jan  8 04:28:42 2027 GMT
  host: fieldtranscript.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FieldTranscript Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FieldTranscript, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: FieldTranscript
provider_slug: fieldtranscript-com
slug: fieldtranscript-com-domain-security
source_filename: fieldtranscript-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fieldtranscript.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 04:28:42 2027 GMT\n  hsts: null\ndomains:\n- domain: fieldtranscript.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/fieldtranscript-com/security/fieldtranscript-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Transcription
- Privacy
- Audio
- Software-as-a-Service
- Individual
---
