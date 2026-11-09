---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: bordeaux.guru
  spf: true
hosts:
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: bordeaux.guru
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bordeaux Guru Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for bordeaux.guru, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: bordeaux.guru
provider_slug: bordeaux-guru
slug: bordeaux-guru-domain-security
source_filename: bordeaux-guru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bordeaux.guru\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: bordeaux.guru\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/bordeaux-guru/security/bordeaux-guru-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Wine
- Vintage
- En Primeur
- Data
- Analytics
- Company
---
