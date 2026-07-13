---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: quera.com
  spf: true
hosts:
- cert_expires: Sep  1 15:47:34 2026 GMT
  host: www.quera.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 22:56:19 2026 GMT
  host: bloqade.quera.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quera Computing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for QuEra Computing, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: QuEra Computing
provider_slug: quera-computing
slug: quera-computing-domain-security
source_filename: quera-computing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.quera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 15:47:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: bloqade.quera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 22:56:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: quera.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quera-computing/refs/heads/main/security/quera-computing-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Quantum Computing
- Neutral Atom
- Analog Hamiltonian Simulation
- AWS Braket
- Aquila
- Gemini
- Fault Tolerance
- Quantum Error Correction
- Bloqade
- Hardware
---
