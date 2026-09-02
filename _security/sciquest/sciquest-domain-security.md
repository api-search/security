---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: jaggaer.com
  spf: true
hosts:
- cert_expires: Oct 10 04:03:34 2026 GMT
  host: www.jaggaer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: asodocs.jaggaer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sciquest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SciQuest, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: SciQuest
provider_slug: sciquest
slug: sciquest-domain-security
source_filename: sciquest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jaggaer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 04:03:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: asodocs.jaggaer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jaggaer.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sciquest/refs/heads/main/security/sciquest-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Enterprise Software
- Procurement
- eProcurement
- Spend Management
- Source-to-Pay
- Supplier Management
- Sourcing
---
