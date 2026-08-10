---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dmarc_rua: mailto:dmarc@execonline.com
  dnssec: false
  domain: execonline.com
  spf: true
  spf_record: v=spf1 include:_spf.execonline.com -all
hosts:
- cert_expires: Sep 21 07:00:32 2026 GMT
  host: www.execonline.com
  hsts: false
  hsts_max_age: null
  https: true
  role: marketing site (WordPress)
  tls_version: TLSv1.3
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: platform.execonline.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_preload: true
  https: true
  role: learning platform (credentialed SPA)
  tls_version: TLSv1.3
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: app.execonline.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_preload: true
  https: true
  role: learning platform (credentialed SPA, alternate host)
  tls_version: TLSv1.3
- cert_expires: Sep 23 05:23:02 2026 GMT
  host: status.execonline.com
  hsts: true
  hsts_max_age: 259200
  https: true
  role: status page (Atlassian Statuspage, vendor-hosted)
  tls_version: TLSv1.3
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: support.execonline.com
  hsts: false
  hsts_max_age: null
  https: true
  role: help center (Intercom, vendor-hosted)
  tls_version: TLSv1.3
- cert_expires: Oct 20 14:25:18 2026 GMT
  host: connect.execonline.com
  hsts: false
  hsts_max_age: null
  https: true
  role: ExecConnect community site (WordPress)
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Execonline Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ExecOnline, probed live across 6 host(s) and 1 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ExecOnline
provider_slug: execonline
slug: execonline-domain-security
source_filename: execonline-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts (probe-domain-security.py, extended\n  by hand to the remaining live execonline.com hosts discovered during contract discovery)\nhosts:\n- host: www.execonline.com\n  role: marketing site (WordPress)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 07:00:32 2026 GMT\n  hsts: false\n  hsts_max_age: null\n- host: platform.execonline.com\n  role: learning platform (credentialed SPA)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  hsts_preload: true\n- host: app.execonline.com\n  role: learning platform (credentialed SPA, alternate host)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  hsts_preload: true\n- host: status.execonline.com\n  role: status page (Atlassian\
  \ Statuspage, vendor-hosted)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 05:23:02 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: support.execonline.com\n  role: help center (Intercom, vendor-hosted)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: false\n  hsts_max_age: null\n- host: connect.execonline.com\n  role: ExecConnect community site (WordPress)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 14:25:18 2026 GMT\n  hsts: false\n  hsts_max_age: null\ndomains:\n- domain: execonline.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.execonline.com -all\n  dmarc: true\n  dmarc_policy: none\n  dmarc_rua: mailto:dmarc@execonline.com\nnotes:\n- 'api.execonline.com resolves to GitHub Pages (185.199.108.153) and returns an unconfigured\n  GitHub Pages HTML page with HTTP 200 for every path probed, including /openapi.json\n  and /.well-known/*. It is a catch-all false positive,\
  \ not an API host.'\n- 'No HSTS on the marketing site (www) or the ExecConnect community site; the credentialed\n  learning-platform hosts do carry a two-year preloaded HSTS policy.'\n- 'DMARC is published at p=none (monitor only) with aggregate and forensic reporting;\n  no CAA records are published; the zone is not DNSSEC-signed.'\nx-evidence:\n  probed: '2026-08-04'\n  method: openssl s_client, curl -I, dig\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/execonline/refs/heads/main/security/execonline-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Education
- Leadership Development
- Executive Education
- Corporate Learning
- Learning and Development
- EdTech
- Coaching
- Talent Development
- Human Resources
- SaaS
---
