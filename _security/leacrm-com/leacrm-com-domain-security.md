---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: leacrm.com
  spf: true
hosts:
- cert_expires: Dec 27 23:38:59 2026 GMT
  host: leacrm.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lea CRM Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lea CRM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Lea CRM
provider_slug: leacrm-com
slug: leacrm-com-domain-security
source_filename: leacrm-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: leacrm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:38:59 2026 GMT\n  hsts: false\ndomains:\n- domain: leacrm.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/leacrm-com/security/leacrm-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- CRM
- Sales
- European
- Software-as-a-Service
- Automation
---
