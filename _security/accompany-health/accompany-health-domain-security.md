---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: accompanyhealth.com
  spf: true
hosts:
- cert_expires: Oct 10 06:24:42 2026 GMT
  cert_issuer: GoDaddy TLS Intermediate CA DV - R1v1
  host: accompanyhealth.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
  waf: Sucuri/Cloudproxy
- cert_expires: Oct 10 06:24:42 2026 GMT
  host: www.accompanyhealth.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  note: redirects to the apex host
  tls_version: TLSv1.3
  waf: Sucuri/Cloudproxy
- host: pay.accompanyhealth.com
  hsts: false
  https: true
  note: Third-party hosted payment link (GoDaddy/Poynt paylinks). Not operated by Accompany Health and not an API surface.
- host: whitepaper.accompanyhealth.com
  hsts: false
  https: true
  note: Static marketing microsite hosting a downloadable white paper.
kind: domain-security
layout: security
method: probed
name: Accompany Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Accompany Health, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Accompany Health
provider_slug: accompany-health
slug: accompany-health-domain-security
source_filename: accompany-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts + certificate-transparency subdomains\nnote: >-\n  The automated probe recorded hsts:null for www.accompanyhealth.com because the\n  Sucuri Cloudproxy WAF in front of the site answers an unsolved request with a 307\n  JavaScript challenge. A hand-probe of the response headers on both the apex and the\n  www host shows HSTS is in fact served (max-age=31536000; includeSubdomains; preload),\n  and that value is recorded here. The two additional hosts were found in\n  certificate-transparency logs (crt.sh) rather than in apis.yml, since this company\n  publishes no API and therefore has no baseURL or servers[] hosts.\nhosts:\n- host: accompanyhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 06:24:42 2026 GMT\n  cert_issuer: GoDaddy TLS Intermediate CA DV - R1v1\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  waf:\
  \ Sucuri/Cloudproxy\n- host: www.accompanyhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 06:24:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  waf: Sucuri/Cloudproxy\n  note: redirects to the apex host\n- host: pay.accompanyhealth.com\n  https: true\n  hsts: false\n  note: >-\n    Third-party hosted payment link (GoDaddy/Poynt paylinks). Not operated by\n    Accompany Health and not an API surface.\n- host: whitepaper.accompanyhealth.com\n  https: true\n  hsts: false\n  note: Static marketing microsite hosting a downloadable white paper.\ndomains:\n- domain: accompanyhealth.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accompany-health/refs/heads/main/security/accompany-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Primary Care
- Home Health
- Telehealth
- Behavioral Health
- Value-Based Care
- Medicaid
- Medicare
- HIPAA
---
