---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: duetti.co
  spf: true
hosts:
- cert_expires: Sep 17 04:20:37 2026 GMT
  host: www.duetti.co
  hsts: null
  https: true
  note: marketing site (Webflow); no HSTS header observed
  tls_version: TLSv1.3
- cert_expires: Oct 17 04:59:07 2026 GMT
  host: duo.duetti.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  note: DUO artist onboarding application; authenticated, 307 redirects all paths to /login
  tls_version: TLSv1.3
- cert_expires: Oct 15 08:31:57 2026 GMT
  host: statements.duetti.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  note: Artist File Vault (royalty statements); authenticated
  tls_version: TLSv1.3
- cert_expires: Oct 30 21:15:55 2026 GMT
  host: sync.duetti.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  note: Sync licensing portal; authenticated
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Duetti Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Duetti, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Duetti
provider_slug: duetti
slug: duetti-domain-security
source_filename: duetti-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.duetti.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 04:20:37 2026 GMT\n  hsts: null\n  note: marketing site (Webflow); no HSTS header observed\n- host: duo.duetti.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 04:59:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  note: DUO artist onboarding application; authenticated, 307 redirects all paths to /login\n- host: statements.duetti.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 08:31:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  note: Artist File Vault (royalty statements); authenticated\n- host: sync.duetti.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 21:15:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  note: Sync licensing portal; authenticated\ndomains:\n- domain: duetti.co\n  dnssec: false\n  caa: []\n\
  \  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/duetti/refs/heads/main/security/duetti-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Music
- Music Rights
- Royalties
- Catalog Acquisition
- Music Finance
- Publishing
- Distribution
- Creator Economy
- Entertainment
---
