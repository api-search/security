---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_note: DMARC record published but policy is p=none — monitoring only, no enforcement against spoofed mail.
  dmarc_policy: none
  dnssec: false
  domain: aavantgarde.com
  spf: true
hosts:
- cert_expires: Oct  8 22:33:42 2026 GMT
  content_security_policy: true
  csp_note: CSP is present but permissive — default-src *, script-src 'self' 'unsafe-inline' 'unsafe-eval' *.
  edge: cloudflare
  host: www.aavantgarde.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  referrer_policy: same-origin
  tls_version: TLSv1.3
  x_content_type_options: nosniff
  x_frame_options: SAMEORIGIN
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aavantgardebio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AAVantgarde Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AAVantgarde Bio
provider_slug: aavantgardebio
slug: aavantgardebio-domain-security
source_filename: aavantgardebio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: >-\n  Live DNS/TLS/HTTP probes of the hosts this record knows on 2026-09-05. AAVantgarde\n  publishes no API, so the only hosts in scope are the corporate site and its\n  registrable domain; api./developer./docs./status./trust. subdomains all NXDOMAIN.\nnote: >-\n  The origin sits behind Cloudflare and answered our probe IP with HTTP 403 \"Sorry, you\n  have been blocked\" on most HTML paths, so header values below were read from the\n  response headers Cloudflare still returned (HSTS is set on the 403 as well as on the\n  200 homepage). /.well-known/* paths were served normally.\nhosts:\n- host: www.aavantgarde.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 22:33:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  x_content_type_options: nosniff\n  x_frame_options: SAMEORIGIN\n  referrer_policy: same-origin\n  content_security_policy: true\n  csp_note:\
  \ >-\n    CSP is present but permissive — default-src *, script-src 'self' 'unsafe-inline'\n    'unsafe-eval' *.\n  edge: cloudflare\ndomains:\n- domain: aavantgarde.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dmarc_note: >-\n    DMARC record published but policy is p=none — monitoring only, no enforcement\n    against spoofed mail.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aavantgardebio/refs/heads/main/security/aavantgardebio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Gene Therapy
- Life Sciences
- Pharmaceuticals
- Clinical Trials
- Ophthalmology
- Rare Disease
- Healthcare
- Italy
---
