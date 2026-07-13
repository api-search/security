---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:support@transloadit.com"
  - 0 issue "amazon.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: transloadit.com
  spf: true
hosts:
- cert_expires: Sep 15 09:19:23 2026 GMT
  host: transloadit.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 26 14:02:22 2026 GMT
  host: api2.transloadit.com
  hsts: true
  hsts_max_age: 15552001
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Transloadit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transloadit, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Transloadit
provider_slug: transloadit
slug: transloadit-domain-security
source_filename: transloadit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: transloadit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 09:19:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api2.transloadit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 26 14:02:22 2026 GMT\n  hsts: true\n  hsts_max_age: 15552001\ndomains:\n- domain: transloadit.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:support@transloadit.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transloadit/refs/heads/main/security/transloadit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- File Processing
- Media Encoding
- Video Transcoding
- Image Resizing
- Audio Extraction
- Thumbnail Generation
- File Uploading
- Media API
---
