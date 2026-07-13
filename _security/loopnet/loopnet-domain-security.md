---
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: loopnet.com
  spf: true
hosts:
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: www.loopnet.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: api.loopnet.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Loopnet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LoopNet, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: LoopNet
provider_slug: loopnet
slug: loopnet-domain-security
source_filename: loopnet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.loopnet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: null\n- host: api.loopnet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: loopnet.com\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loopnet/refs/heads/main/security/loopnet-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Commercial Real Estate
- Property Listings
- CRE
- Real Estate
- Market Analytics
- CoStar
- Lease Rates
- Sale Comparables
---
