---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mozonic.com
  spf: true
hosts:
- cert_expires: May 30 09:48:24 2027 GMT
  host: mozonic.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mozonic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mozonic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mozonic
provider_slug: mozonic-com
slug: mozonic-com-domain-security
source_filename: mozonic-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mozonic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May 30 09:48:24 2027 GMT\n  hsts: false\ndomains:\n- domain: mozonic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mozonic-com/security/mozonic-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Audio
- Artificial Intelligence
- Music Production
- Digital Audio Workstation
- Mix Analysis
---
