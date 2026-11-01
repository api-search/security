---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: insuremo.com
  spf: true
hosts:
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: insuremo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Insuremo Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for InsureMo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: InsureMo
provider_slug: insuremo-com
slug: insuremo-com-domain-security
source_filename: insuremo-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: insuremo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: insuremo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/insuremo-com/security/insuremo-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Insurance
- AI
- Platform
- API
---
