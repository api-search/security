---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: staffeto.com
  spf: true
hosts:
- cert_expires: Oct 31 14:25:16 2026 GMT
  host: staffeto.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Staffeto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Staffeto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Staffeto
provider_slug: staffeto
slug: staffeto-domain-security
source_filename: staffeto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: staffeto.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 31 14:25:16 2026 GMT\n  hsts: null\ndomains:\n- domain: staffeto.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/staffeto/security/staffeto-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Workforce
- Automation
- Scheduling
- HR
---
