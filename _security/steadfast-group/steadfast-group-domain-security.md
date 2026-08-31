---
api_specs:
- filename: steadfast-group-address-api-openapi.yml
  format: yaml
  label: Steadfast Group Address API
  slug: steadfast-group-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steadfast-group/refs/heads/main/openapi/steadfast-group-address-api-openapi.yml
- filename: steadfast-group-risk-api-openapi.yml
  format: yaml
  label: Steadfast Group Risk API
  slug: steadfast-group-risk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steadfast-group/refs/heads/main/openapi/steadfast-group-risk-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: steadfast.com.au
  note: DMARC is at p=reject with aggregate and forensic reporting via vali.email - a strong email posture.
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: steadfastagencies.com.au
  spf: true
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: steadfastlife.com.au
  note: The only Steadfast domain with DNSSEC signing and CAA records - and it is a divisional site, not the primary domain. The divergence suggests it sits with a different registrar/host than the corporate estate.
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: steadfastnz.nz
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: steadfast.com.sg
  spf: true
hosts:
- cert_expires: Sep 11 16:10:21 2026 GMT
  host: www.steadfast.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  role: Corporate and consumer marketing site
  tls_version: TLSv1.3
- cert_expires: Oct  2 14:58:09 2026 GMT
  host: floodrisktracker.steadfast.com.au
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 2592000
  hsts_preload: false
  https: true
  note: 30-day HSTS max-age, below the one-year threshold required for preload eligibility. Fronted by Cloudflare. Additional response headers observed - x-content-type-options nosniff, x-frame-options sameorigin, x-xss-protection 1; mode=block, and x-powered-by ASP.NET, which discloses the server stack unnecessarily.
  role: Public Flood Risk Tracker tool and the estate's only public API
  tls_version: TLSv1.2
- cert_expires: Oct 22 11:49:51 2026 GMT
  host: idp.steadfast.com.au
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 315360000
  https: true
  note: Ten-year HSTS with includeSubDomains - the strongest transport posture in the estate.
  role: Okta-hosted OpenID Connect identity provider
  tls_version: TLSv1.2
- cert_expires: Oct 13 08:47:31 2026 GMT
  host: broker.steadfast.com.au
  hsts: false
  https: true
  note: No Strict-Transport-Security header on the login wall used by 414 member brokerages. This is the most consequential gap found in the estate.
  role: Credentialed broker portal (Optimizely/Episerver DXP)
  tls_version: TLSv1.3
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: api.steadfast.com.au
  hsts: false
  https: true
  role: Undocumented partner API host (403 at root)
  tls_version: TLSv1.2
- cert_expires: Sep 17 23:59:59 2026 GMT
  host: api-sf.steadfast.com.au
  hsts: false
  https: true
  role: Partner API host discovered via certificate transparency (403 at root)
  tls_version: TLSv1.3
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: investor.steadfast.com.au
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  role: Investor relations platform (third party)
  tls_version: TLSv1.3
- cert_expires: Sep 27 01:47:09 2026 GMT
  host: steadfastagencies.com.au
  hsts: true
  hsts_max_age: 2592000
  https: true
  role: Steadfast Underwriting Agencies
  tls_version: TLSv1.2
- cert_expires: Sep  7 00:51:27 2026 GMT
  host: www.steadfastlife.com.au
  hsts: true
  hsts_max_age: 63072000
  https: true
  role: Steadfast Life
  tls_version: TLSv1.3
- cert_expires: Sep 10 06:27:31 2026 GMT
  host: www.steadfastnz.nz
  hsts: true
  hsts_max_age: 31536000
  https: true
  role: Steadfast New Zealand
  tls_version: TLSv1.3
- cert_expires: Sep 12 01:55:40 2026 GMT
  host: www.steadfast.com.sg
  hsts: true
  hsts_max_age: 31536000
  https: true
  role: Steadfast Singapore
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Steadfast Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Steadfast Group, probed live across 11 host(s) and 5 registrable domain(s). 11 host(s) serve HTTPS (up to TLSv1.3); 8 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Steadfast Group
provider_slug: steadfast-group
slug: steadfast-group-domain-security
source_filename: steadfast-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: >-\n  live DNS/TLS/HTTP probes of every Steadfast Group host in apis.yml, the OpenAPI servers, and\n  the additional hosts discovered through certificate transparency, run 2026-07-25\nhosts:\n- host: www.steadfast.com.au\n  role: Corporate and consumer marketing site\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 16:10:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: floodrisktracker.steadfast.com.au\n  role: Public Flood Risk Tracker tool and the estate's only public API\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  2 14:58:09 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n  hsts_include_subdomains: false\n  hsts_preload: false\n  note: >-\n    30-day HSTS max-age, below the one-year threshold required for preload eligibility. Fronted\n    by Cloudflare. Additional response headers observed - x-content-type-options nosniff,\n    x-frame-options sameorigin, x-xss-protection 1; mode=block,\
  \ and x-powered-by ASP.NET, which\n    discloses the server stack unnecessarily.\n- host: idp.steadfast.com.au\n  role: Okta-hosted OpenID Connect identity provider\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 22 11:49:51 2026 GMT\n  hsts: true\n  hsts_max_age: 315360000\n  hsts_include_subdomains: true\n  note: Ten-year HSTS with includeSubDomains - the strongest transport posture in the estate.\n- host: broker.steadfast.com.au\n  role: Credentialed broker portal (Optimizely/Episerver DXP)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 08:47:31 2026 GMT\n  hsts: false\n  note: >-\n    No Strict-Transport-Security header on the login wall used by 414 member brokerages. This is\n    the most consequential gap found in the estate.\n- host: api.steadfast.com.au\n  role: Undocumented partner API host (403 at root)\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: false\n- host: api-sf.steadfast.com.au\n  role: Partner API\
  \ host discovered via certificate transparency (403 at root)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:59:59 2026 GMT\n  hsts: false\n- host: investor.steadfast.com.au\n  role: Investor relations platform (third party)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n- host: steadfastagencies.com.au\n  role: Steadfast Underwriting Agencies\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 27 01:47:09 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: www.steadfastlife.com.au\n  role: Steadfast Life\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 00:51:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.steadfastnz.nz\n  role: Steadfast New Zealand\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 06:27:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.steadfast.com.sg\n\
  \  role: Steadfast Singapore\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 01:55:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: steadfast.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  note: DMARC is at p=reject with aggregate and forensic reporting via vali.email - a strong email posture.\n- domain: steadfastagencies.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: steadfastlife.com.au\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy:\
  \ quarantine\n  note: >-\n    The only Steadfast domain with DNSSEC signing and CAA records - and it is a divisional site,\n    not the primary domain. The divergence suggests it sits with a different registrar/host than\n    the corporate estate.\n- domain: steadfastnz.nz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: steadfast.com.sg\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\nfindings:\n- >-\n  Email authentication is consistently strong: SPF everywhere and DMARC at p=reject on four of\n  five domains - a meaningful control for a broker network exposed to invoice and premium fraud.\n- >-\n  DNSSEC and CAA are absent on the primary steadfast.com.au domain and on every domain except\n  steadfastlife.com.au. Nothing constrains which certificate authority may issue for the\n  corporate or API hosts.\n- >-\n  HSTS is inconsistent across the estate, ranging from ten years with includeSubDomains on the\n  identity\
  \ provider to entirely absent on the broker login wall and both partner API hosts.\n- >-\n  Two hosts still negotiate TLS 1.2 as their top protocol, including the public API host and the\n  identity provider.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/steadfast-group/refs/heads/main/security/steadfast-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Insurance
- Australia
- Brokers
- Insurance Broker Network
- General Insurance
- Property and Casualty
- Underwriting Agency
- Agency Management
- ACORD
- Partner Gated
- New Zealand
---
