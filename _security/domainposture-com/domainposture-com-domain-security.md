---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: domainposture.com
  spf: true
hosts:
- cert_expires: Jan  9 20:34:37 2027 GMT
  host: domainposture.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Domainposture Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Domain Posture, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Domain Posture
provider_slug: domainposture-com
slug: domainposture-com-domain-security
source_filename: domainposture-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: domainposture.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 20:34:37 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: domainposture.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/domainposture-com/security/domainposture-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Security
- Domain
- Monitoring
---
