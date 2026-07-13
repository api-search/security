---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: secondspectrum.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: geniussports.com
  spf: true
hosts:
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: www.secondspectrum.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Mar 19 23:59:59 2027 GMT
  host: performancestudio.geniussports.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: geniussports.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Second Spectrum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Second Spectrum (Genius Sports), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Second Spectrum (Genius Sports)
provider_slug: second-spectrum
slug: second-spectrum-domain-security
source_filename: second-spectrum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.secondspectrum.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: null\n- host: performancestudio.geniussports.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 19 23:59:59 2027 GMT\n  hsts: null\n- host: geniussports.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: secondspectrum.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: geniussports.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/second-spectrum/refs/heads/main/security/second-spectrum-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Sports Tracking
- Computer Vision
- AI
- Broadcast
- NBA
- Premier League
- Genius Sports
- Performance Studio
- Skeletal Tracking
- Optical Tracking
- Augmented Broadcast
---
