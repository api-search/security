---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getamplifylife.com
  spf: true
hosts:
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: getamplifylife.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: api.getamplifylife.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amplify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amplify, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Amplify
provider_slug: amplify
slug: amplify-domain-security
source_filename: amplify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getamplifylife.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: false\n- host: api.getamplifylife.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: getamplifylife.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amplify/refs/heads/main/security/amplify-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Insurance
- Insurtech
- Life Insurance
- Financial Services
- Fintech
- Embedded Finance
- Annuities
---
