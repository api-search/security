---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: namebrewery.com
  spf: true
hosts:
- cert_expires: Jan 11 01:18:32 2027 GMT
  host: namebrewery.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Name Brewery Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Name Brewery, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Name Brewery
provider_slug: namebrewery-com
slug: namebrewery-com-domain-security
source_filename: namebrewery-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: namebrewery.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 01:18:32 2027 GMT\n  hsts: false\ndomains:\n- domain: namebrewery.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/namebrewery-com/security/namebrewery-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Domain
- Naming
- Tool
---
