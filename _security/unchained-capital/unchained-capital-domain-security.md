---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: unchained.com
  spf: true
hosts:
- cert_expires: Sep 13 17:38:16 2026 GMT
  host: www.unchained.com
  hsts: false
  https: true
  role: marketing site
  tls_version: TLSv1.3
- cert_expires: Sep 20 18:48:19 2026 GMT
  host: my.unchained.com
  hsts: true
  hsts_max_age: 0
  https: true
  note: Strict-Transport-Security present but max-age=0, which disables HSTS.
  role: client application (login/sign-up)
  tls_version: TLSv1.3
- cert_expires: Sep 19 23:13:48 2026 GMT
  host: help.unchained.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  role: knowledge base (HubSpot-hosted)
  tls_version: TLSv1.3
- cert_expires: Oct 26 17:49:19 2026 GMT
  host: status.unchained.com
  hsts: true
  hsts_max_age: 63113904
  https: true
  role: status page (Better Stack) — SSO-gated, redirects to /sso; not public
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unchained Capital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unchained Capital, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Unchained Capital
provider_slug: unchained-capital
slug: unchained-capital-domain-security
source_filename: unchained-capital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unchained.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 17:38:16 2026 GMT\n  hsts: false\n  role: marketing site\n- host: my.unchained.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 18:48:19 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n  role: client application (login/sign-up)\n  note: Strict-Transport-Security present but max-age=0, which disables HSTS.\n- host: help.unchained.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:13:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  role: knowledge base (HubSpot-hosted)\n- host: status.unchained.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 17:49:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63113904\n  role: status page (Better Stack) — SSO-gated, redirects to /sso; not public\ndomains:\n- domain: unchained.com\n  dnssec: true\n\
  \  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unchained-capital/refs/heads/main/security/unchained-capital-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Bitcoin
- Cryptocurrency
- Financial-Services
- Custody
- Wealth Management
- Lending
- Retirement
- Trading
- Open-Source
---
