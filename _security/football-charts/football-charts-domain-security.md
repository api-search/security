---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: football-charts.com
  spf: true
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:security+caafailure@render.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: onrender.com
  spf: false
hosts:
- cert_expires: Oct 26 15:29:17 2026 GMT
  host: www.football-charts.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 21:54:17 2026 GMT
  host: footballcharts-backend.onrender.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 13:36:21 2026 GMT
  host: mcp.football-charts.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Football Charts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Football Charts, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Football Charts
provider_slug: football-charts
slug: football-charts-domain-security
source_filename: football-charts-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.football-charts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 15:29:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: footballcharts-backend.onrender.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 21:54:17 2026 GMT\n  hsts: false\n- host: mcp.football-charts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 13:36:21 2026 GMT\n  hsts: false\ndomains:\n- domain: football-charts.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: onrender.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:security+caafailure@render.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: false\n  dmarc:\
  \ true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/football-charts/refs/heads/main/security/football-charts-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- football
- soccer
- sports
- sports-data
- statistics
- results
- standings
- fixtures
- predictions
- probability-models
- monte-carlo
- mcp
- agent-native
- free-api
---
