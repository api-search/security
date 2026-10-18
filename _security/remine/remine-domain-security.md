---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: remine.com
  spf: true
hosts:
- cert_expires: Dec 24 19:57:20 2026 GMT
  host: remine.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Remine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Remine, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Remine
provider_slug: remine
slug: remine-domain-security
source_filename: remine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: remine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 19:57:20 2026 GMT\n  hsts: false\ndomains:\n- domain: remine.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/remine/refs/heads/main/security/remine-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Real Estate
- Property Data
- Mortgage Data
- Lead Generation
- Predictive Analytics
- MLS
---
