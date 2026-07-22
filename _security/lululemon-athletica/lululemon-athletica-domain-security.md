---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:caaalerts@lululemon.com"
  - 0 issue "globalsign.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lululemon.com
  spf: true
hosts:
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: shop.lululemon.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lululemon Athletica Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lululemon Athletica, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lululemon Athletica
provider_slug: lululemon-athletica
slug: lululemon-athletica-domain-security
source_filename: lululemon-athletica-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shop.lululemon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: lululemon.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:caaalerts@lululemon.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lululemon-athletica/refs/heads/main/security/lululemon-athletica-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Apparel
- Athletic Wear
- Retail
- Ecommerce
- Fortune 500
---
