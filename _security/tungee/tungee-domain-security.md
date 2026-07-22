---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tungee.com
  spf: true
hosts:
- cert_expires: Sep 21 23:59:59 2026 GMT
  host: www.tungee.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Tungee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tungee, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Tungee
provider_slug: tungee
slug: tungee-domain-security
source_filename: tungee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tungee.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 21 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: tungee.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tungee/refs/heads/main/security/tungee-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Sales Intelligence
- CRM
- Lead Generation
- AI Agents
- B2B Data
- China
---
