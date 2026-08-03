---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: teikametrics.com
  spf: true
hosts:
- cert_expires: Oct  2 19:38:45 2026 GMT
  host: www.teikametrics.com
  hsts: false
  https: true
  role: website
  tls_version: TLSv1.3
- cert_expires: Oct 26 23:59:59 2026 GMT
  host: help.teikametrics.com
  hsts: false
  https: true
  note: Intercom-hosted help centre (CNAME d3noi0rmtp7b0c.cloudfront.net).
  role: documentation
  tls_version: TLSv1.3
- cert_expires: Oct 26 23:59:59 2026 GMT
  host: app.teikametrics.com
  hsts: false
  https: true
  note: CloudFront-fronted SPA (app.production.teikametrics.com).
  role: application
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Teikametrics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Teikametrics, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Teikametrics
provider_slug: teikametrics
slug: teikametrics-domain-security
source_filename: teikametrics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.teikametrics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 19:38:45 2026 GMT\n  hsts: false\n  role: website\n- host: help.teikametrics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 23:59:59 2026 GMT\n  hsts: false\n  role: documentation\n  note: Intercom-hosted help centre (CNAME d3noi0rmtp7b0c.cloudfront.net).\n- host: app.teikametrics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 23:59:59 2026 GMT\n  hsts: false\n  role: application\n  note: CloudFront-fronted SPA (app.production.teikametrics.com).\nfindings:\n- No HSTS on any Teikametrics host (website, help centre or application).\n- No CAA record on teikametrics.com — certificate issuance is unrestricted.\n- DNSSEC not enabled on teikametrics.com.\n- DMARC present but at p=quarantine rather than p=reject.\n- No API host exists — api./developer./docs.teikametrics.com\
  \ are all NXDOMAIN.\ndomains:\n- domain: teikametrics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teikametrics/refs/heads/main/security/teikametrics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Advertising
- Retail
- E-Commerce
- Marketplaces
- Artificial Intelligence
- Analytics
- Amazon
- Walmart
- Inventory
---
