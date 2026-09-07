---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: acelerate.io
  spf: true
hosts:
- cert_expires: Oct 21 21:23:27 2026 GMT
  host: acelerate.io
  hsts: true
  hsts_max_age: 15724800
  https: true
  note: Apex; 301 redirects to app.acelerate.io. The Webflow marketing site that ran here was retired (last archived 2023-10-04).
  tls_version: TLSv1.3
- cert_expires: Oct 21 21:23:27 2026 GMT
  host: app.acelerate.io
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15724800
  https: true
  note: 'The only origin-serving host on the estate. Fronted by Cloudflare with a bot challenge (cf-mitigated: challenge, HTTP 403) on HTML and /api/* paths; /robots.txt and /.well-known/* pass through to the origin. acelerate.io and www.acelerate.io 301 here.'
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Acelerate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acelerate, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Acelerate
provider_slug: acelerate
slug: acelerate-domain-security
source_filename: acelerate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts, plus app.acelerate.io -- the production application host named\n  by WEB_URL/API_URL_IN_BROWSER in the shipped Next.js bundle (STEP 0b contract discovery)\nhosts:\n- host: acelerate.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 21:23:27 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n  note: Apex; 301 redirects to app.acelerate.io. The Webflow marketing site that ran here was retired (last archived\n    2023-10-04).\n- host: app.acelerate.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 21:23:27 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n  hsts_include_subdomains: true\n  note: 'The only origin-serving host on the estate. Fronted by Cloudflare with a bot challenge (cf-mitigated: challenge,\n    HTTP 403) on HTML and /api/* paths; /robots.txt and /.well-known/* pass through to the origin. acelerate.io\n    and www.acelerate.io 301 here.'\n\
  domains:\n- domain: acelerate.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acelerate/refs/heads/main/security/acelerate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Restaurants
- Restaurant Technology
- Food Service
- Hospitality
- Ghost Kitchens
- Supply Chain
- Procurement
- Foodservice Distribution
- SaaS
- United States
- Company
---
