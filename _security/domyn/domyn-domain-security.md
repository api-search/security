---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: domyn.com
  spf: true
hosts:
- cert_expires: Dec 13 21:12:40 2026 GMT
  host: www.domyn.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Domyn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Domyn, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Domyn
provider_slug: domyn
slug: domyn-domain-security
source_filename: domyn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.domyn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 21:12:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: domyn.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/domyn/security/domyn-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Enterprise
- Platform
- Automation
- Regulated Industries
---
