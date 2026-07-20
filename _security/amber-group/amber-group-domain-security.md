---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ambergroup.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ambr.io
  spf: true
hosts:
- cert_expires: Sep 16 22:27:46 2026 GMT
  host: www.ambergroup.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 23:59:59 2026 GMT
  host: www.ambr.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amber Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amber Group, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amber Group
provider_slug: amber-group
slug: amber-group-domain-security
source_filename: amber-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ambergroup.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 22:27:46 2026 GMT\n  hsts: false\n- host: www.ambr.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: ambergroup.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: ambr.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amber-group/refs/heads/main/security/amber-group-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Cryptocurrency
- Digital Assets
- Trading
- Asset Management
- Wealth Management
- Institutional
- Blockchain
- API
---
