---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazontrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zoey.com
  spf: true
hosts:
- cert_expires: Jan 16 21:46:40 2027 GMT
  host: zoey.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Zoey Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zoey, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zoey
provider_slug: zoey
slug: zoey-domain-security
source_filename: zoey-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zoey.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 21:46:40 2027 GMT\n  hsts: false\ndomains:\n- domain: zoey.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/zoey/security/zoey-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- B2B
- Ecommerce
- Wholesale
- Integration
---
