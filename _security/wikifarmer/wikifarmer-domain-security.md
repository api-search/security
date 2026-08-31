---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wikifarmer.com
  spf: true
hosts:
- cert_expires: Sep 15 15:13:04 2026 GMT
  host: wikifarmer.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wikifarmer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wikifarmer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Wikifarmer
provider_slug: wikifarmer
slug: wikifarmer-domain-security
source_filename: wikifarmer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wikifarmer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 15:13:04 2026 GMT\n  hsts: false\ndomains:\n- domain: wikifarmer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wikifarmer/refs/heads/main/security/wikifarmer-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Agriculture
- Agtech
- Marketplace
- Farming
- B2B
- Education
- Commodities
- Price Data
- Sustainability
---
