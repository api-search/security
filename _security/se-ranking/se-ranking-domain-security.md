---
api_specs:
- filename: overview
  format: yaml
  label: SE Ranking Data API
  slug: data-api
  spec_type: Postman
  url: https://www.postman.com/serankingdev/se-ranking-developers/overview
- filename: overview
  format: yaml
  label: SE Ranking Project API
  slug: project-api
  spec_type: Postman
  url: https://www.postman.com/serankingdev/se-ranking-developers/overview
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: seranking.com
  spf: true
hosts:
- cert_expires: Aug 14 19:05:08 2026 GMT
  host: seranking.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  8 23:26:51 2026 GMT
  host: api.seranking.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Se Ranking Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SE Ranking, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SE Ranking
provider_slug: se-ranking
slug: se-ranking-domain-security
source_filename: se-ranking-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: seranking.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 19:05:08 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: api.seranking.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  8 23:26:51 2026 GMT\n  hsts: null\ndomains:\n- domain: seranking.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/se-ranking/refs/heads/main/security/se-ranking-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SEO
- Keyword Research
- Rank Tracking
- Backlinks
- Competitor Analysis
- Website Audit
- AI Search
- GEO
- Digital Marketing
---
