---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: augmedix.com
  spf: true
hosts:
- cert_expires: Sep 28 19:23:26 2026 GMT
  host: www.augmedix.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 23:59:59 2026 GMT
  host: ee-portal.augmedix.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Augmedix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Augmedix, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Augmedix
provider_slug: augmedix
slug: augmedix-domain-security
source_filename: augmedix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.augmedix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 19:23:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ee-portal.augmedix.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 15 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: augmedix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/augmedix/refs/heads/main/security/augmedix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Medical Documentation
- AI Scribe
- Ambient AI
- Clinical Notes
- EHR Integration
- Epic
- Cerner
- Athenahealth
- HIPAA
- HITRUST
- Commure
- Health Technology
---
