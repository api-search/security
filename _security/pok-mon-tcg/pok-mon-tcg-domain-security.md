---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pokemontcg.io
  spf: true
hosts:
- cert_expires: Oct  8 08:30:14 2026 GMT
  host: pokemontcg.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pok Mon Tcg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pokémon TCG, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Pokémon TCG
provider_slug: pok-mon-tcg
slug: pok-mon-tcg-domain-security
source_filename: pok-mon-tcg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pokemontcg.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 08:30:14 2026 GMT\n  hsts: false\ndomains:\n- domain: pokemontcg.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pok-mon-tcg/refs/heads/main/security/pok-mon-tcg-domain-security.yml
summary_line: TLSv1.3
tags:
- Games And Comics
- Public APIs
---
