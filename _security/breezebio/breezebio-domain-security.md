---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: breezebio.com
  spf: true
hosts:
- cert_expires: Oct 21 09:43:15 2026 GMT
  host: breezebio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Breezebio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Breezebio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Breezebio
provider_slug: breezebio
slug: breezebio-domain-security
source_filename: breezebio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: breezebio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 09:43:15 2026 GMT\n  hsts: false\ndomains:\n- domain: breezebio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/breezebio/refs/heads/main/security/breezebio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Genetic Medicine
- Drug Delivery
- Therapeutics
- Life Sciences
- Nanoparticles
- Healthcare
---
