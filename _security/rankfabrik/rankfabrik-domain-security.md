---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rankfabrik.com
  spf: true
hosts:
- cert_expires: Nov 15 11:23:32 2026 GMT
  host: rankfabrik.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 11:23:32 2026 GMT
  host: places.rankfabrik.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 11:23:32 2026 GMT
  host: jobs.rankfabrik.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Rankfabrik Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RankFabrik, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: RankFabrik
provider_slug: rankfabrik
slug: rankfabrik-domain-security
source_filename: rankfabrik-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rankfabrik.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 11:23:32 2026 GMT\n  hsts: false\n- host: places.rankfabrik.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 11:23:32 2026 GMT\n  hsts: null\n- host: jobs.rankfabrik.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 11:23:32 2026 GMT\n  hsts: null\ndomains:\n- domain: rankfabrik.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rankfabrik/refs/heads/main/security/rankfabrik-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Data
- Web Scraping
- Local Business
- Places
- Job
- Job Postings
- video-transcripts
- Captions
- Email Verification
- Data Enrichment
- Lead Generation
- REST API
---
