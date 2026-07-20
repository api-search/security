---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: incorta.com
  spf: true
hosts:
- cert_expires: Aug 25 01:34:46 2026 GMT
  host: incorta.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Incorta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Incorta, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Incorta
provider_slug: incorta
slug: incorta-domain-security
source_filename: incorta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: incorta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 01:34:46 2026 GMT\n  hsts: false\ndomains:\n- domain: incorta.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/incorta/refs/heads/main/security/incorta-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Enterprise
- Analytics
- Business Intelligence
- Data Platform
- Data Analytics
- Data Integration
- Dashboards
---
