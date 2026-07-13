---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gouv.fr
  spf: false
hosts:
- cert_expires: Aug 10 08:00:34 2026 GMT
  host: geo.api.gouv.fr
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: French Address Search Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for French Address Search, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: French Address Search
provider_slug: french-address-search
slug: french-address-search-domain-security
source_filename: french-address-search-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: geo.api.gouv.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 08:00:34 2026 GMT\n  hsts: false\ndomains:\n- domain: gouv.fr\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/french-address-search/refs/heads/main/security/french-address-search-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Open Data
- Public APIs
---
