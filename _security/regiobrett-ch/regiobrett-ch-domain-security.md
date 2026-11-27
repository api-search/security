---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dns_aid:
    checked: '2026-11-22'
    published: false
  dnssec: true
  domain: regiobrett.ch
  spf: true
hosts:
- cert_expires: Jan 25 09:14:05 2027 GMT
  host: regiobrett.ch
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Witzelfitz Consulting GmbH Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Witzelfitz Consulting GmbH, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Witzelfitz Consulting GmbH
provider_slug: regiobrett-ch
slug: regiobrett-ch-domain-security
source_filename: regiobrett-ch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: regiobrett.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 09:14:05 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: regiobrett.ch\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dns_aid:\n    checked: '2026-11-22'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/regiobrett-ch/security/regiobrett-ch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- DigitalPinboard
- Community
- Switzerland
- Ostschweiz
---
