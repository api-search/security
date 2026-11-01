---
api_specs:
- filename: scrapewhale-dev-openapi.json
  format: json
  label: ScrapeWhale API
  slug: scrapewhale-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scrapewhale-dev/openapi/scrapewhale-dev-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: scrapewhale.dev
  spf: true
hosts:
- cert_expires: Jan 12 06:32:06 2027 GMT
  host: scrapewhale.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Scrapewhale Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for scrapewhale-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: scrapewhale-dev
provider_slug: scrapewhale-dev
slug: scrapewhale-dev-domain-security
source_filename: scrapewhale-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scrapewhale.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 06:32:06 2027 GMT\n  hsts: false\ndomains:\n- domain: scrapewhale.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/scrapewhale-dev/security/scrapewhale-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Data
- Marketing
- API
- WebScraping
- AI
---
