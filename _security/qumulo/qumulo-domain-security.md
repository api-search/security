---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: qumulo.com
  spf: true
hosts:
- cert_expires: Aug 27 18:26:25 2026 GMT
  host: qumulo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 19:47:17 2026 GMT
  host: docs.qumulo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qumulo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qumulo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Qumulo
provider_slug: qumulo
slug: qumulo-domain-security
source_filename: qumulo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: qumulo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 18:26:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.qumulo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 19:47:17 2026 GMT\n  hsts: false\ndomains:\n- domain: qumulo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qumulo/refs/heads/main/security/qumulo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Storage
- File Storage
- Data Platform
- Cloud Storage
- Unstructured Data
- Enterprise
- Infrastructure
- REST API
- CLI
---
