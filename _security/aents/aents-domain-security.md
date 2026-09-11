---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aents.co
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aentscope.com
  note: SPF delegates mail to Cloudflare (include:_spf.mx.cloudflare.net ~all); DMARC is published in monitor-only mode (p=none, rua=dmarc@aentscope.com). No CAA record and no DS record, so certificate issuance is unconstrained and the zone is unsigned.
  spf: true
hosts:
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: aents.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 15:18:12 2026 GMT
  host: www.aentscope.com
  hsts: false
  https: true
  note: AENTSCOPE tenant application (Next.js on Vercel); root is the sign-in screen.
  tls_version: TLSv1.3
- host: docs.aentscope.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  note: GitBook space behind Cloudflare; answers HTTP 401 on every path, so only the TLS and header layer is observable anonymously.
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Aents Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AENTS, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AENTS
provider_slug: aents
slug: aents-domain-security
source_filename: aents-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\n# probe-domain-security.py covers the apis.yml Website host only; the two aentscope.com\n# hosts (the AENTSCOPE application and its GitBook docs space) were probed by hand on\n# 2026-09-10 with openssl s_client, curl -I and dig, and are recorded below with the\n# same fields.\nhosts:\n- host: aents.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: false\n- host: www.aentscope.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 15:18:12 2026 GMT\n  hsts: false\n  note: AENTSCOPE tenant application (Next.js on Vercel); root is the sign-in screen.\n- host: docs.aentscope.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 63072000\n  note: >-\n    GitBook space behind Cloudflare; answers HTTP 401 on every path, so only the TLS\n    and header layer is observable anonymously.\ndomains:\n- domain: aents.co\n\
  \  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: aentscope.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  note: >-\n    SPF delegates mail to Cloudflare (include:_spf.mx.cloudflare.net ~all); DMARC is\n    published in monitor-only mode (p=none, rua=dmarc@aentscope.com). No CAA record and\n    no DS record, so certificate issuance is unconstrained and the zone is unsigned.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aents/refs/heads/main/security/aents-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Climate Tech
- Carbon Accounting
- Carbon Management
- ESG
- Sustainability
- Greenhouse Gas
- Net Zero
- Emissions Reporting
- SaaS
- South Korea
---
