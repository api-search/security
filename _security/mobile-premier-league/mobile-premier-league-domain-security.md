---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mplgames.com
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: mpl.live
  spf: true
  spf_record: v=spf1 include:_spf.google.com ~all
hosts:
- cert_expires: Nov  9 13:57:52 2026 GMT
  host: www.mplgames.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: www.mpl.live
  hsts: false
  https: true
- host: api.mpl.live
  hsts: false
  https: true
kind: domain-security
layout: security
method: probed
name: Mobile Premier League Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mobile Premier League, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Mobile Premier League
provider_slug: mobile-premier-league
slug: mobile-premier-league-domain-security
source_filename: mobile-premier-league-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the Mobile Premier League consumer + API hosts\nnote: >-\n  www.mplgames.com is the live consumer surface; www.mpl.live is the legacy India surface and\n  api.mpl.live is the app-facing gateway (returns JSON 404s to every unauthenticated path).\n  Both apex domains were probed even though only mplgames.com is wired as a pointer in apis.yml.\nhosts:\n- host: www.mplgames.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 13:57:52 2026 GMT\n  hsts: false\n- host: www.mpl.live\n  https: true\n  hsts: false\n- host: api.mpl.live\n  https: true\n  hsts: false\ndomains:\n- domain: mplgames.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: mpl.live\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com ~all\n  dmarc: false\nfindings:\n- id: no-dmarc\n  severity: medium\n  detail: Neither mplgames.com nor mpl.live publishes a _dmarc TXT\
  \ record.\n- id: no-spf-mplgames\n  severity: medium\n  detail: mplgames.com publishes no SPF record; mpl.live publishes v=spf1 include:_spf.google.com ~all.\n- id: no-caa\n  severity: low\n  detail: No CAA records on either apex domain.\n- id: no-hsts\n  severity: low\n  detail: No Strict-Transport-Security header on www.mplgames.com, www.mpl.live or api.mpl.live.\n- id: dangling-cname\n  severity: high\n  detail: >-\n    developer.mpl.live is a CNAME to\n    dualstack.prod-developer-dashboard-2060818981.ap-south-1.elb.amazonaws.com, which itself\n    returns NXDOMAIN. The record points at a deleted AWS load balancer — the classic\n    subdomain-takeover shape. Reported here as an observed DNS fact, not as an exploit.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mobile-premier-league/refs/heads/main/security/mobile-premier-league-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Gaming
- Mobile Gaming
- Esports
- Skill Gaming
- Games
- Consumer
- Entertainment
- Tournaments
- India
---
