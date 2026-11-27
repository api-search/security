---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: familyguy.co.uk
  spf: true
hosts:
- cert_expires: Jan 30 22:41:09 2027 GMT
  host: familyguy.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Family Guy Episode Database Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Family Guy Episode Database, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Family Guy Episode Database
provider_slug: familyguy-co-uk
slug: familyguy-co-uk-domain-security
source_filename: familyguy-co-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: familyguy.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 22:41:09 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: familyguy.co.uk\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/familyguy-co-uk/security/familyguy-co-uk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Entertainment
- Television
- Database
- Community
---
