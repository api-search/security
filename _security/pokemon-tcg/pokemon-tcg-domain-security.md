---
api_specs:
- filename: pokemon-tcg-openapi.yml
  format: yaml
  label: Pokémon TCG Cards API
  slug: pokemon-tcg-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pokemon-tcg/refs/heads/main/openapi/pokemon-tcg-openapi.yml
- filename: pokemon-tcg-openapi.yml
  format: yaml
  label: Pokémon TCG Sets API
  slug: pokemon-tcg-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pokemon-tcg/refs/heads/main/openapi/pokemon-tcg-openapi.yml
- filename: pokemon-tcg-openapi.yml
  format: yaml
  label: Pokémon TCG Metadata API
  slug: pokemon-tcg-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pokemon-tcg/refs/heads/main/openapi/pokemon-tcg-openapi.yml
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
- cert_expires: Oct  8 08:30:14 2026 GMT
  host: docs.pokemontcg.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 08:30:14 2026 GMT
  host: api.pokemontcg.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pokemon Tcg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pokémon TCG API, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Pokémon TCG API
provider_slug: pokemon-tcg
slug: pokemon-tcg-domain-security
source_filename: pokemon-tcg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pokemontcg.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 08:30:14 2026 GMT\n  hsts: false\n- host: docs.pokemontcg.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 08:30:14 2026 GMT\n  hsts: false\n- host: api.pokemontcg.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 08:30:14 2026 GMT\n  hsts: null\ndomains:\n- domain: pokemontcg.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pokemon-tcg/refs/heads/main/security/pokemon-tcg-domain-security.yml
summary_line: TLSv1.3
tags:
- Pokemon
- Trading Cards
- TCG
- Gaming
- Card Games
- Collectibles
- Card Prices
---
