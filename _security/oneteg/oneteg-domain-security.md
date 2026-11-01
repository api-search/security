---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: oneteg.com
  spf: true
hosts:
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: oneteg.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Oneteg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CyanGate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: CyanGate
provider_slug: oneteg
slug: oneteg-domain-security
source_filename: oneteg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oneteg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: oneteg.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/oneteg/security/oneteg-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- API Security
- Gateways
- Enterprise
- Cloud Integration
- Monitoring
---
