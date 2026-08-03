---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aescape.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: zitadel.cloud
  note: third-party identity platform domain hosting the Aescape tenant, recorded for completeness — not under Aescape control
  spf: true
hosts:
- cert_expires: Sep 26 05:05:49 2026 GMT
  host: www.aescape.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  role: marketing site (Vercel / Next.js)
  tls_version: TLSv1.3
- cert_expires: Feb 10 23:59:59 2027 GMT
  host: app.aescape.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  role: consumer booking application (Flutter web SPA)
  tls_version: TLSv1.3
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: api.aescape.com
  hsts: false
  https: true
  role: private application API host (AWS API Gateway; apigw-requestid header present, every probed path returns 404 {"message":"Not Found"})
  tls_version: TLSv1.3
- cert_expires: Oct 20 22:37:19 2026 GMT
  host: developer.aescape.com
  hsts: false
  https: true
  role: developer documentation site, gated behind HTTP Basic auth (WWW-Authenticate; realm "Developer Docs", fronted by Cloudflare) — returns 401 on every path
  tls_version: TLSv1.3
- cert_expires: Oct  4 08:14:02 2026 GMT
  host: store.aescape.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  role: Shopify storefront (gifts and packages)
  tls_version: TLSv1.3
- cert_expires: Oct 22 01:31:45 2026 GMT
  host: aescape-8ocoec.zitadel.cloud
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_preload: true
  https: true
  role: Aescape production identity tenant (Zitadel), serves the OpenID Connect discovery document
  third_party_domain: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aescape Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aescape, probed live across 6 host(s) and 2 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Aescape
provider_slug: aescape
slug: aescape-domain-security
source_filename: aescape-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts + hosts observed in the app.aescape.com\n  Content-Security-Policy\nhosts:\n- host: www.aescape.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 05:05:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  role: marketing site (Vercel / Next.js)\n- host: app.aescape.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  role: consumer booking application (Flutter web SPA)\n- host: api.aescape.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: false\n  role: private application API host (AWS API Gateway; apigw-requestid header present,\n    every probed path returns 404 {\"message\":\"Not Found\"})\n- host: developer.aescape.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 22:37:19 2026 GMT\n  hsts: false\n\
  \  role: developer documentation site, gated behind HTTP Basic auth (WWW-Authenticate;\n    realm \"Developer Docs\", fronted by Cloudflare) — returns 401 on every path\n- host: store.aescape.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 08:14:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n  role: Shopify storefront (gifts and packages)\n- host: aescape-8ocoec.zitadel.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 01:31:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  role: Aescape production identity tenant (Zitadel), serves the OpenID Connect discovery\n    document\n  third_party_domain: true\ndomains:\n- domain: aescape.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: zitadel.cloud\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  note: third-party identity platform domain hosting the Aescape tenant,\
  \ recorded for\n    completeness — not under Aescape control\nnotes:\n- No CAA records are published on aescape.com.\n- DNSSEC is not enabled on aescape.com.\n- No /.well-known/security.txt was served on any Aescape host (see well-known/aescape-well-known.yml).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aescape/refs/heads/main/security/aescape-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Robotics
- Health and Wellness
- Fitness
- Massage
- Artificial Intelligence
- Consumer Hardware
- Hospitality
- Recovery
- Identity
---
