---
api_specs:
- filename: madeonsol-robinhood-chain-api-openapi.yml
  format: yaml
  label: MadeOnSol Robinhood Chain API
  slug: madeonsol-robinhood-chain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/madeonsol/refs/heads/main/openapi/madeonsol-robinhood-chain-api-openapi.yml
- filename: madeonsol-solana-api-openapi.yml
  format: yaml
  label: MadeOnSol Solana API
  slug: madeonsol-solana-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/madeonsol/refs/heads/main/openapi/madeonsol-solana-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:info@madeonsol.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: madeonsol.com
  spf: true
hosts:
- cert_expires: Dec 15 10:59:15 2026 GMT
  host: madeonsol.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Madeonsol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MadeOnSol, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: MadeOnSol
provider_slug: madeonsol
slug: madeonsol-domain-security
source_filename: madeonsol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: madeonsol.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 10:59:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: madeonsol.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:info@madeonsol.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/madeonsol/refs/heads/main/security/madeonsol-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- Analytics
- Solana
- Robinhood Chain
- API
---
