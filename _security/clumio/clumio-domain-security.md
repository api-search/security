---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: clumio.com
  spf: true
hosts:
- cert_expires: Sep 27 17:59:47 2026 GMT
  host: clumio.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- host: developers.clumio.com
  https: false
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: us-west-2.api.clumio.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clumio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clumio, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Clumio
provider_slug: clumio
slug: clumio-domain-security
source_filename: clumio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clumio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 17:59:47 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: developers.clumio.com\n  https: false\n- host: us-west-2.api.clumio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: clumio.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clumio/refs/heads/main/security/clumio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Data
- Backup
- Data Protection
- Disaster Recovery
- Cloud
- Storage
- Security
- Compliance
---
