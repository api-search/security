---
description: ''
domains:
- caa: []
  caa_note: No CAA record published — any public CA may issue for this domain.
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: lovebonito.com
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:spf.mandrillapp.com include:servers.mcsv.net include:mail.zendesk.com ~all
hosts:
- cert_expires: Oct 12 19:56:19 2026 GMT
  host: www.lovebonito.com
  hsts: max-age=31536000; includeSubDomains
  hsts_max_age: 31536000
  https: true
  note: Storefront is a Next.js app served through Cloudflare. HSTS is present on every response, including the WAF block pages. Cloudflare began answering 403 to repeated automated GETs partway through the pass, so some probe rows below record a challenge rather than an origin response.
  tls_version: TLSv1.3
- cert_expires: Oct 12 19:56:19 2026 GMT
  cert_issuer: Google Trust Services WE1
  host: api.lovebonito.com
  hsts: max-age=31536000; includeSubDomains
  hsts_max_age: 31536000
  https: true
  note: First-party Kong API gateway (x-kong-response-latency header) fronted by Cloudflare. Every path probed returned HTTP 401 {"message":"Unauthorized"}. Not a published/documented API — it serves Love, Bonito's own storefront and mobile apps.
  tls_version: TLSv1.3
- host: admin.lovebonito.com
  hsts: max-age=31536000; includeSubDomains
  https: true
  note: Administrative host; returns a Cloudflare 403 to anonymous requests.
kind: domain-security
layout: security
method: probed
name: Love Bonito Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Love Bonito, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Love Bonito
provider_slug: love-bonito
slug: love-bonito-domain-security
source_filename: love-bonito-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of lovebonito.com hosts (probe-domain-security.py + manual curl, 2026-08-25)\nhosts:\n- host: www.lovebonito.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 19:56:19 2026 GMT\n  hsts: max-age=31536000; includeSubDomains\n  hsts_max_age: 31536000\n  note: >-\n    Storefront is a Next.js app served through Cloudflare. HSTS is present on every response,\n    including the WAF block pages. Cloudflare began answering 403 to repeated automated GETs\n    partway through the pass, so some probe rows below record a challenge rather than an origin\n    response.\n- host: api.lovebonito.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 19:56:19 2026 GMT\n  cert_issuer: Google Trust Services WE1\n  hsts: max-age=31536000; includeSubDomains\n  hsts_max_age: 31536000\n  note: >-\n    First-party Kong API gateway (x-kong-response-latency header) fronted by Cloudflare. Every\n    path\
  \ probed returned HTTP 401 {\"message\":\"Unauthorized\"}. Not a published/documented API —\n    it serves Love, Bonito's own storefront and mobile apps.\n- host: admin.lovebonito.com\n  https: true\n  hsts: max-age=31536000; includeSubDomains\n  note: Administrative host; returns a Cloudflare 403 to anonymous requests.\ndomains:\n- domain: lovebonito.com\n  dnssec: true\n  caa: []\n  caa_note: No CAA record published — any public CA may issue for this domain.\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com include:spf.mandrillapp.com include:servers.mcsv.net include:mail.zendesk.com ~all\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/love-bonito/refs/heads/main/security/love-bonito-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Retail
- E-Commerce
- Fashion
- Apparel
- Direct to Consumer
- Singapore
- Southeast Asia
---
