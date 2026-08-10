---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: crowdstreet.com
  spf: true
hosts:
- cert_expires: Oct 21 05:35:35 2026 GMT
  host: crowdstreet.com
  hsts: false
  hsts_max_age: null
  https: true
  role: marketing site (Framer-hosted)
  tls_version: TLSv1.3
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: app2.crowdstreet.com
  hsts: false
  hsts_max_age: null
  http_status: 200
  https: true
  role: investor web application (SPA)
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: api.crowdstreet.com
  hsts: false
  hsts_max_age: null
  http_status: 403
  https: true
  role: private backend API (AWS API Gateway; unauthenticated requests return '{"message":"Missing Authentication Token"}')
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: help.crowdstreet.com
  hsts: true
  hsts_max_age: 2592000
  http_status: 200
  https: true
  role: help center / education center
  server: Microsoft-IIS/10.0
kind: domain-security
layout: security
method: probed
name: Crowdstreet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CrowdStreet, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CrowdStreet
provider_slug: crowdstreet
slug: crowdstreet-domain-security
source_filename: crowdstreet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts (0-working/probe-domain-security.py,\n  plus manual probes of the app/API/help hosts, which are not reachable from apis.yml\n  link properties alone)\nhosts:\n- host: crowdstreet.com\n  role: marketing site (Framer-hosted)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 05:35:35 2026 GMT\n  hsts: false\n  hsts_max_age: null\n- host: app2.crowdstreet.com\n  role: investor web application (SPA)\n  https: true\n  http_status: 200\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: false\n  hsts_max_age: null\n- host: api.crowdstreet.com\n  role: private backend API (AWS API Gateway; unauthenticated requests return '{\"message\":\"Missing\n    Authentication Token\"}')\n  https: true\n  http_status: 403\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: false\n  hsts_max_age: null\n- host: help.crowdstreet.com\n  role: help center / education center\n  https: true\n  http_status:\
  \ 200\n  server: Microsoft-IIS/10.0\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: crowdstreet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\nnotes:\n- HSTS is absent on the marketing site, the investor application and the API host;\n  only help.crowdstreet.com sets Strict-Transport-Security (max-age 2592000, 30 days,\n  below the 31536000 commonly required for preload).\n- No CAA records and no DNSSEC on crowdstreet.com.\n- DMARC is published but the policy is p=none (monitor only), so spoofed mail is not\n  rejected or quarantined.\n- 'Wildcard DNS caveat: status., trust., support., developer. and docs.crowdstreet.com\n  all resolve and return the same 858-byte investor-portal SPA shell. These are catch-all\n  responses, not real status/trust/developer surfaces, and must not be scored as such.'\nx-evidence:\n  fetched: '2026-08-04'\n  method: curl HEAD/GET + openssl s_client + dig\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crowdstreet/refs/heads/main/security/crowdstreet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real Estate
- Commercial Real Estate
- Investing
- Private Markets
- Alternative Investments
- Crowdfunding
- Financial Services
- FinTech
- Wealth Management
---
