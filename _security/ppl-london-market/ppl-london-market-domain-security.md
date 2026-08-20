---
api_specs:
- filename: ppl-london-market-placements.json
  format: json
  label: PPL Placements API
  slug: ppl-placements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-placements.json
- filename: ppl-london-market-submissions.json
  format: json
  label: PPL Submissions API
  slug: ppl-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-submissions.json
- filename: ppl-london-market-organisations.json
  format: json
  label: PPL Organisations API
  slug: ppl-organisations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-organisations.json
- filename: ppl-london-market-documents.json
  format: json
  label: PPL Documents API
  slug: ppl-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-documents.json
- filename: ppl-london-market-events.json
  format: json
  label: PPL Events API
  slug: ppl-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/openapi/ppl-london-market-events.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: placingplatformlimited.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pplnextgen.com
  spf: true
hosts:
- cert_expires: Sep  3 14:24:46 2026 GMT
  host: placingplatformlimited.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: developer.pplnextgen.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: api.londonmarketgroup.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ppl London Market Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PPL, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PPL
provider_slug: ppl-london-market
slug: ppl-london-market-domain-security
source_filename: ppl-london-market-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: placingplatformlimited.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 14:24:46 2026 GMT\n  hsts: false\n- host: developer.pplnextgen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api.londonmarketgroup.co.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: placingplatformlimited.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: pplnextgen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ppl-london-market/refs/heads/main/security/ppl-london-market-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- United Kingdom
- London Market
- Lloyd's of London
- Reinsurance
- Commercial Insurance
- Brokers
- Underwriting
- Placement
- Market Infrastructure
- ACORD
- Electronic Placing
---
