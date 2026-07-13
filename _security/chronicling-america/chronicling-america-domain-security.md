---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: loc.gov
  spf: true
hosts:
- cert_expires: Sep 13 04:56:11 2026 GMT
  host: chroniclingamerica.loc.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chronicling America Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chronicling America, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Chronicling America
provider_slug: chronicling-america
slug: chronicling-america-domain-security
source_filename: chronicling-america-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chroniclingamerica.loc.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 04:56:11 2026 GMT\n  hsts: null\ndomains:\n- domain: loc.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chronicling-america/refs/heads/main/security/chronicling-america-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- News
- Public APIs
---
