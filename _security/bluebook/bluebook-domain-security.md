---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getbluebook.com
  spf: true
hosts:
- cert_expires: Aug 25 13:29:40 2026 GMT
  cert_issuer: Let's Encrypt E8
  host: getbluebook.com
  hsts: true
  hsts_max_age: 31536000
  http_status: 404
  https: true
  note: Apex resolves and terminates TLS correctly with HSTS, but the Framer-hosted marketing site returned HTTP 404 for every path probed on 2026-07-20 (/, /about, /security, /blog, /pricing, /privacy, /terms, /careers, /login, /contact). The Internet Archive's last successful capture is 2026-04-16. The site appears unpublished or mid-migration rather than the domain lost.
  server: Framer
  tls_version: TLSv1.3
- cert_expires: May 18 18:34:29 2026 GMT
  cert_issuer: Let's Encrypt R12
  host: agent.getbluebook.com
  hosting: Vercel
  http_status: 404
  https: false
  https_error: certificate expired
  note: Application host referenced by the archived site's "Log in" link (https://agent.getbluebook.com/login). TLS certificate expired 2026-05-18, so the host fails verification; with verification disabled it returns 404.
- host: api.getbluebook.com
  hosting: Render (CNAME bluebook-api.onrender.com)
  https: false
  https_error: TLS handshake failed
  note: DNS still delegates this host to Render, but the TLS handshake fails entirely, consistent with a deleted or suspended service behind a stale DNS record. No API surface was reachable.
kind: domain-security
layout: security
method: probed
name: Bluebook Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bluebook, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bluebook
provider_slug: bluebook
slug: bluebook-domain-security
source_filename: bluebook-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getbluebook.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: \"Let's Encrypt E8\"\n  cert_expires: Aug 25 13:29:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  http_status: 404\n  server: Framer\n  note: >-\n    Apex resolves and terminates TLS correctly with HSTS, but the Framer-hosted\n    marketing site returned HTTP 404 for every path probed on 2026-07-20\n    (/, /about, /security, /blog, /pricing, /privacy, /terms, /careers, /login,\n    /contact). The Internet Archive's last successful capture is 2026-04-16.\n    The site appears unpublished or mid-migration rather than the domain lost.\n- host: agent.getbluebook.com\n  https: false\n  https_error: certificate expired\n  cert_issuer: \"Let's Encrypt R12\"\n  cert_expires: May 18 18:34:29 2026 GMT\n  http_status: 404\n  hosting: Vercel\n  note: >-\n    Application host referenced by the\
  \ archived site's \"Log in\" link\n    (https://agent.getbluebook.com/login). TLS certificate expired\n    2026-05-18, so the host fails verification; with verification disabled it\n    returns 404.\n- host: api.getbluebook.com\n  https: false\n  https_error: TLS handshake failed\n  hosting: Render (CNAME bluebook-api.onrender.com)\n  note: >-\n    DNS still delegates this host to Render, but the TLS handshake fails\n    entirely, consistent with a deleted or suspended service behind a stale\n    DNS record. No API surface was reachable.\ndomains:\n- domain: getbluebook.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluebook/refs/heads/main/security/bluebook-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Accounting
- Artificial Intelligence
- AI Agents
- Financial Close
- Bookkeeping
- Sweden
---
