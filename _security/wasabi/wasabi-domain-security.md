---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wasabi.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wasabisys.com
  spf: false
hosts:
- cert_expires: Sep  8 14:04:09 2026 GMT
  host: wasabi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 01:12:03 2026 GMT
  host: docs.wasabi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 23:59:59 2026 GMT
  host: s3.wasabisys.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wasabi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wasabi, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wasabi
provider_slug: wasabi
slug: wasabi-domain-security
source_filename: wasabi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wasabi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 14:04:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.wasabi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 01:12:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: s3.wasabisys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wasabi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: wasabisys.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wasabi/refs/heads/main/security/wasabi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Storage
- Object Storage
- S3 Compatible
- REST API
- Hot Storage
- Buckets
- Objects
- Media Storage
- Backup
- Enterprise Storage
---
