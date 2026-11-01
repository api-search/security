---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: psnc.pl
  spf: true
hosts:
- cert_expires: Dec 12 12:48:05 2026 GMT
  host: www.psnc.pl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Psnc Pl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Institute of Bioorganic Chemistry of the Polish Academy of Sciences - Poznan Supercomputing and Networking Center, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Institute of Bioorganic Chemistry of the Polish Academy of Sciences - Poznan Supercomputing and Networking Center
provider_slug: psnc-pl
slug: psnc-pl-domain-security
source_filename: psnc-pl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.psnc.pl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 12:48:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: psnc.pl\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/psnc-pl/security/psnc-pl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Research
- Supercomputing
- Networking
- Poland
- Science
---
