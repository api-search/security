---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: audiblemagic.com
  spf: true
hosts:
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: audiblemagic.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Audible Magic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Audible Magic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Audible Magic
provider_slug: audible-magic
slug: audible-magic-domain-security
source_filename: audible-magic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: audiblemagic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: audiblemagic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/audible-magic/security/audible-magic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Automatic Content Recognition
- Content Identification
- Rights Management
- Music Licensing
- Copyright Compliance
- Audio Fingerprinting
---
