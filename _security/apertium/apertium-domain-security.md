---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apertium.org
  spf: true
hosts:
- cert_expires: Dec 29 10:55:04 2026 GMT
  host: apertium.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Apertium Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apertium, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Apertium
provider_slug: apertium
slug: apertium-domain-security
source_filename: apertium-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apertium.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 10:55:04 2026 GMT\n  hsts: false\ndomains:\n- domain: apertium.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/apertium/security/apertium-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Machine Translation
- Open Source
- Linguistics
- Natural Language Processing
- Community
---
