---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: interweave.biz
  spf: true
hosts:
- cert_expires: Dec 12 23:05:24 2026 GMT
  host: interweave.biz
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Interweave Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for InterWevae Smart Solutions, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: InterWevae Smart Solutions
provider_slug: interweave
slug: interweave-domain-security
source_filename: interweave-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: interweave.biz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:05:24 2026 GMT\n  hsts: false\ndomains:\n- domain: interweave.biz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/interweave/security/interweave-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Integration
- CRM
- ERP
- Automation
---
