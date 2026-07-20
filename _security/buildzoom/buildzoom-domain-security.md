---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: buildzoom.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: buildzoomdata.com
  spf: true
hosts:
- cert_expires: Sep  9 05:42:25 2026 GMT
  host: www.buildzoom.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: www.buildzoomdata.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: api.buildzoomdata.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Buildzoom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BuildZoom, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BuildZoom
provider_slug: buildzoom
slug: buildzoom-domain-security
source_filename: buildzoom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.buildzoom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 05:42:25 2026 GMT\n  hsts: false\n- host: www.buildzoomdata.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: false\n- host: api.buildzoomdata.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: buildzoom.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: buildzoomdata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buildzoom/refs/heads/main/security/buildzoom-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Construction
- Building Permits
- Contractors
- Real Estate
- Home Improvement
- Property Data
- Marketplace
---
