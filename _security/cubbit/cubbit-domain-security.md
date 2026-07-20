---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cubbit.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cubbit.eu
  spf: true
hosts:
- cert_expires: Sep 23 16:15:11 2026 GMT
  host: cubbit.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: docs.cubbit.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 11:56:25 2026 GMT
  host: s3.cubbit.eu
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cubbit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cubbit, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cubbit
provider_slug: cubbit
slug: cubbit-domain-security
source_filename: cubbit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cubbit.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 16:15:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.cubbit.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: false\n- host: s3.cubbit.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 11:56:25 2026 GMT\n  hsts: null\ndomains:\n- domain: cubbit.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: cubbit.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cubbit/refs/heads/main/security/cubbit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Object Storage
- Cloud Storage
- S3 Compatible
- Storage
- Data Sovereignty
- Geo-Distributed
- Infrastructure
- Company
---
