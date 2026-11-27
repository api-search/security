---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ihateaudio.com
  spf: true
hosts:
- cert_expires: Dec 21 11:47:47 2026 GMT
  host: ihateaudio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ihateaudio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ihateaudio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ihateaudio
provider_slug: ihateaudio-com
slug: ihateaudio-com-domain-security
source_filename: ihateaudio-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ihateaudio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 11:47:47 2026 GMT\n  hsts: false\ndomains:\n- domain: ihateaudio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/ihateaudio-com/security/ihateaudio-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Audio
- Tools
- Browser
- Free
- Open Source
- Privacy
---
