---
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "geotrust.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: league.com
  spf: true
hosts:
- cert_expires: Oct 23 06:41:09 2026 GMT
  host: league.com
  hsts: null
  hsts_note: 'NOT observed. A 200 GET of https://league.com/robots.txt returned no Strict-Transport-Security header (server: cloudflare). The marketing origin does not set HSTS even though the API and app hosts do.'
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 08:06:38 2026 GMT
  host: api.league.com
  hsts: max-age=31536000; includeSubDomains; preload
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_note: Observed directly on a live GET https://api.league.com/ (2026-08-25). The automated probe recorded null because the host answers 404 on /; the header is present regardless of status.
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
- host: app.league.com
  hsts: max-age=31536000; includeSubDomains
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_note: Observed on a live 200 GET (2026-08-25). Added by hand — not in apis.yml hosts at probe time.
  hsts_preload: false
  https: true
kind: domain-security
layout: security
method: probed
name: League Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for League, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: League
provider_slug: league
slug: league-domain-security
source_filename: league-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: league.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 06:41:09 2026 GMT\n  hsts: null\n  hsts_note: 'NOT observed. A 200 GET of https://league.com/robots.txt returned no Strict-Transport-Security\n    header (server: cloudflare). The marketing origin does not set HSTS even though the API and app hosts\n    do.'\n- host: api.league.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 08:06:38 2026 GMT\n  hsts: max-age=31536000; includeSubDomains; preload\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  hsts_note: Observed directly on a live GET https://api.league.com/ (2026-08-25). The automated probe\n    recorded null because the host answers 404 on /; the header is present regardless of status.\n- host: app.league.com\n  https: true\n  hsts: max-age=31536000; includeSubDomains\n  hsts_max_age:\
  \ 31536000\n  hsts_include_subdomains: true\n  hsts_preload: false\n  hsts_note: Observed on a live 200 GET (2026-08-25). Added by hand — not in apis.yml hosts at probe time.\ndomains:\n- domain: league.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"geotrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\nnote: HSTS values corrected/added from direct header observation on 2026-08-25. DNSSEC is NOT enabled\n  on league.com; CAA, SPF and DMARC are all present, with DMARC at p=reject — a strong email posture.\n  The gap worth naming is DNSSEC, and HSTS missing on the marketing origin while present on api. and app.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/league/refs/heads/main/security/league-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Healthcare
- Digital Health
- Health Benefits
- Interoperability
- FHIR
- Agents
- Artificial Intelligence
- Patient Engagement
- Insurance
- SaaS
---
