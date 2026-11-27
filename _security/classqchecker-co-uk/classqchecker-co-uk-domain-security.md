---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: classqchecker.co.uk
  spf: true
hosts:
- cert_expires: Jan 10 02:09:42 2027 GMT
  host: classqchecker.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Class Q Checker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Class Q Checker, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Class Q Checker
provider_slug: classqchecker-co-uk
slug: classqchecker-co-uk-domain-security
source_filename: classqchecker-co-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: classqchecker.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 02:09:42 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: classqchecker.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/classqchecker-co-uk/security/classqchecker-co-uk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Class Q
- Planning
- United Kingdom
- Real Estate
- Permitted Development
---
