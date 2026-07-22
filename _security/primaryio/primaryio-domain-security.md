---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: primaryio.com
  spf: true
hosts:
- cert_expires: Sep 29 23:28:16 2026 GMT
  host: www.primaryio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Primaryio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PrimaryIO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PrimaryIO
provider_slug: primaryio
slug: primaryio-domain-security
source_filename: primaryio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.primaryio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:28:16 2026 GMT\n  hsts: false\ndomains:\n- domain: primaryio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/primaryio/refs/heads/main/security/primaryio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Big Data
- Disaster Recovery
- Ransomware Recovery
- Cloud Migration
- Data Protection
- VMware
- Cloud
---
