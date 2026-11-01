---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: aplos.com
  spf: true
hosts:
- cert_expires: Dec  6 00:02:19 2026 GMT
  host: www.aplos.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aplos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aplos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Aplos
provider_slug: aplos
slug: aplos-domain-security
source_filename: aplos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aplos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 00:02:19 2026 GMT\n  hsts: false\ndomains:\n- domain: aplos.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/aplos/security/aplos-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Accounting
- Nonprofit
- Software
- Cloud
---
