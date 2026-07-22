---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazonaws.com"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:url@ae.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ae.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: americaneagle.com
  spf: true
hosts:
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: www.ae.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: www.americaneagle.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: American Eagle Outfitters Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for American Eagle Outfitters, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: American Eagle Outfitters
provider_slug: american-eagle-outfitters
slug: american-eagle-outfitters-domain-security
source_filename: american-eagle-outfitters-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ae.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: null\n- host: www.americaneagle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: ae.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:url@ae.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: americaneagle.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/american-eagle-outfitters/refs/heads/main/security/american-eagle-outfitters-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Retail
- E-Commerce
- Fashion
- Apparel
- Consumer Goods
- Fortune 1000
---
