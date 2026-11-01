---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: disa.mil
  spf: true
hosts:
- cert_expires: Dec 15 15:29:27 2026 GMT
  host: www.disa.mil
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Us Dept Of Defense Disa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for US Dept. of Defense/DISA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: US Dept. of Defense/DISA
provider_slug: us-dept-of-defense-disa
slug: us-dept-of-defense-disa-domain-security
source_filename: us-dept-of-defense-disa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.disa.mil\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 15:29:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: disa.mil\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/us-dept-of-defense-disa/security/us-dept-of-defense-disa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Defense
- Government
- Cybersecurity
- IT Services
- Defense
- Government
- Cybersecurity
- IT Services
---
