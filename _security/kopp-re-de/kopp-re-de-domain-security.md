---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kopp-re.de
  spf: true
hosts:
- cert_expires: Dec 22 22:39:48 2026 GMT
  host: kopp-re.de
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kopp Real Estate GmbH Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kopp Real Estate GmbH, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kopp Real Estate GmbH
provider_slug: kopp-re-de
slug: kopp-re-de-domain-security
source_filename: kopp-re-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kopp-re.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 22:39:48 2026 GMT\n  hsts: false\ndomains:\n- domain: kopp-re.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/kopp-re-de/security/kopp-re-de-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Real Estate
- Brokerage
- Munich
- Germany
- Property Services
---
