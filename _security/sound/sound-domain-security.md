---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sound.ag
  spf: true
hosts:
- cert_expires: Oct 20 12:01:47 2026 GMT
  host: www.sound.ag
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sound Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sound Agriculture, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sound Agriculture
provider_slug: sound
slug: sound-domain-security
source_filename: sound-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sound.ag\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 12:01:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sound.ag\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sound/refs/heads/main/security/sound-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Agriculture
- AgTech
- Biologicals
- Crop Nutrition
- Soil Health
- Fertilizer
- Plant Breeding
- Sustainability
---
