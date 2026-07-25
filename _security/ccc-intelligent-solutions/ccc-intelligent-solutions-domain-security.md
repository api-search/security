---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cccis.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cccsecureshare.com
  spf: true
hosts:
- cert_expires: Sep 20 03:17:57 2026 GMT
  host: www.cccis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 11:14:08 2026 GMT
  host: www.cccsecureshare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 03:41:28 2026 GMT
  host: api.cccsecureshare.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: api.cccis.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Production API gateway (Apigee behind Cloudflare); added by hand after the apis.yml pass wired it as a baseURL.
  tls_version: TLSv1.3
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: auth.cccis.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 315360000
  https: true
  note: Okta custom domain. Negotiated TLSv1.2 (ECDHE-RSA-AES128-GCM-SHA256) rather than TLSv1.3 - the only CCC host in this set that does not reach 1.3.
  tls_version: TLSv1.2
- cert_expires: Sep  4 04:13:31 2026 GMT
  host: connect.cccis.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ccc Intelligent Solutions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CCC Intelligent Solutions, probed live across 6 host(s) and 2 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 5 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CCC Intelligent Solutions
provider_slug: ccc-intelligent-solutions
slug: ccc-intelligent-solutions-domain-security
source_filename: ccc-intelligent-solutions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cccis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 03:17:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.cccsecureshare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 11:14:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.cccsecureshare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 03:41:28 2026 GMT\n  hsts: null\n- host: api.cccis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: Production API gateway (Apigee behind Cloudflare); added by hand after the\n    apis.yml pass wired it as a baseURL.\n- host: auth.cccis.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 315360000\n  hsts_include_subdomains:\
  \ true\n  note: Okta custom domain. Negotiated TLSv1.2 (ECDHE-RSA-AES128-GCM-SHA256) rather\n    than TLSv1.3 - the only CCC host in this set that does not reach 1.3.\n- host: connect.cccis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 04:13:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\ndomains:\n- domain: cccis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: cccsecureshare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ccc-intelligent-solutions/refs/heads/main/security/ccc-intelligent-solutions-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- United States
- Property and Casualty
- Claims
- Auto Physical Damage
- Collision Repair
- Insurtech
- Claims Technology
- CIECA
- Partner Gated
- OAuth
- OpenID Connect
---
