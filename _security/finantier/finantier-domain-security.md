---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: finantier.co
  spf: false
hosts:
- cert_expires: Dec  1 22:20:52 2026 GMT
  host: finantier.co
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Finantier Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Finantier, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Finantier
provider_slug: finantier
slug: finantier-domain-security
source_filename: finantier-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: finantier.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 22:20:52 2026 GMT\n  hsts: false\ndomains:\n- domain: finantier.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/finantier/security/finantier-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Finance
- OpenFinance
- SoutheastAsia
- FinTech
---
