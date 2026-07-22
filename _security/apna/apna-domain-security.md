---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: apna.co
  spf: true
hosts:
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: apna.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apna, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Apna
provider_slug: apna
slug: apna-domain-security
source_filename: apna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apna.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: apna.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apna/refs/heads/main/security/apna-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Jobs
- Recruiting
- Professional Networking
- Hiring
- Career
- India
---
