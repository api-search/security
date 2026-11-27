---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: peppol.org
  spf: true
hosts:
- cert_expires: Jan 20 09:48:48 2027 GMT
  host: peppol.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Peppol network (OpenPeppol) Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Peppol network (OpenPeppol), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Peppol network (OpenPeppol)
provider_slug: peppol
slug: peppol-domain-security
source_filename: peppol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: peppol.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 09:48:48 2027 GMT\n  hsts: false\ndomains:\n- domain: peppol.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/peppol/security/peppol-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Peppol
- e-Delivery
- Digital Trade
- Interoperability
- Open Source
---
