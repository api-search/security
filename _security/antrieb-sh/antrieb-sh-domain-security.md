---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: antrieb.sh
  spf: true
hosts:
- cert_expires: Jan 22 08:28:34 2027 GMT
  host: antrieb.sh
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Antrieb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Antrieb, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Antrieb
provider_slug: antrieb-sh
slug: antrieb-sh-domain-security
source_filename: antrieb-sh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: antrieb.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 08:28:34 2027 GMT\n  hsts: false\ndomains:\n- domain: antrieb.sh\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/antrieb-sh/security/antrieb-sh-domain-security.yml
summary_line: TLSv1.3
tags:
- Artificial Intelligence
- Testbeds
- Infrastructure
- Verification
- Cloud
---
