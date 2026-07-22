---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: valyuu.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: valyuu.tech
  spf: true
hosts:
- cert_expires: Aug 31 00:22:33 2026 GMT
  host: valyuu.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 09:25:25 2026 GMT
  host: api-staging.valyuu.tech
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Valyuu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Valyuu, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Valyuu
provider_slug: valyuu
slug: valyuu-domain-security
source_filename: valyuu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: valyuu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 00:22:33 2026 GMT\n  hsts: null\n- host: api-staging.valyuu.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 09:25:25 2026 GMT\n  hsts: null\ndomains:\n- domain: valyuu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: valyuu.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/valyuu/refs/heads/main/security/valyuu-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Recommerce
- Trade-In
- Circular Economy
- Consumer Electronics
- Sustainability
- eCommerce
---
