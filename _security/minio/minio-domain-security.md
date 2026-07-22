---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: min.io
  spf: true
hosts:
- cert_expires: Oct 17 06:59:14 2026 GMT
  host: min.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 01:28:29 2026 GMT
  host: play.min.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Minio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MinIO, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: MinIO
provider_slug: minio
slug: minio-domain-security
source_filename: minio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: min.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 06:59:14 2026 GMT\n  hsts: false\n- host: play.min.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 01:28:29 2026 GMT\n  hsts: null\ndomains:\n- domain: min.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/minio/refs/heads/main/security/minio-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Object Storage
- Storage
- S3 Compatible
- Cloud Native
- Kubernetes
- Data Infrastructure
- AI Storage
- Company
---
