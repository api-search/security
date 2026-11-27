---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: creditgps.ca
  spf: false
hosts:
- cert_expires: Feb  1 11:00:13 2027 GMT
  host: creditgps.ca
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Credit GPS Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Credit GPS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Credit GPS
provider_slug: creditgps-ca
slug: creditgps-ca-domain-security
source_filename: creditgps-ca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: creditgps.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 11:00:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: creditgps.ca\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/creditgps-ca/security/creditgps-ca-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Credit Score
- Personal Finance
- Fintech
- Canada
- Credit Cards
- Financial Education
---
