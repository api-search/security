---
api_specs:
- filename: re-max-eu-datahub-api.postman_collection.json
  format: json
  label: RE/MAX Europe Datahub API
  slug: re-max-eu-datahub-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/re-max/refs/heads/main/collections/re-max-eu-datahub-api.postman_collection.json
- filename: re-max-eu-listings-api.postman_collection.json
  format: json
  label: RE/MAX Europe Listings API
  slug: re-max-eu-listings-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/re-max/refs/heads/main/collections/re-max-eu-listings-api.postman_collection.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: remax.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: remax.eu
  spf: true
hosts:
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: www.remax.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 04:19:21 2026 GMT
  host: www.remax.eu
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 03:54:38 2026 GMT
  host: apidocs.datahub.remax.eu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 22:50:38 2026 GMT
  host: listingsapi-test.datahub.remax.eu
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  note: Postman-hosted documentation; the strongest transport posture in the estate
  tls_version: TLSv1.3
- cert_expires: Oct 12 23:59:59 2026 GMT
  host: api.datahub.remax.eu
  hsts: false
  https: true
  note: the production Datahub API host negotiates TLS 1.2 and sets no HSTS
  tls_version: TLSv1.2
- cert_expires: Oct 12 23:59:59 2026 GMT
  host: oauth.datahub.remax.eu
  hsts: false
  https: true
  note: the OAuth authorization server negotiates TLS 1.2 and sets no HSTS, while also carrying tokens in query strings
  tls_version: TLSv1.2
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: datahub.remax.eu
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: listing-api-remaxeu.bwscloud.tech
  hsts: false
  https: true
  note: staging Listings API on a third-party vendor domain, outside RE/MAX DNS control
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Re Max Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RE/MAX, probed live across 8 host(s) and 2 registrable domain(s). 8 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: RE/MAX
provider_slug: re-max
slug: re-max-domain-security
source_filename: re-max-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.remax.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: null\n- host: www.remax.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 04:19:21 2026 GMT\n  hsts: false\n- host: apidocs.datahub.remax.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 03:54:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: listingsapi-test.datahub.remax.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 22:50:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  note: Postman-hosted documentation; the strongest transport posture in the estate\n- host: api.datahub.remax.eu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 12 23:59:59 2026 GMT\n  hsts: false\n  note: the production Datahub API host negotiates TLS 1.2\
  \ and sets no HSTS\n- host: oauth.datahub.remax.eu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 12 23:59:59 2026 GMT\n  hsts: false\n  note: >-\n    the OAuth authorization server negotiates TLS 1.2 and sets no HSTS, while\n    also carrying tokens in query strings\n- host: datahub.remax.eu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: false\n- host: listing-api-remaxeu.bwscloud.tech\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: false\n  note: staging Listings API on a third-party vendor domain, outside RE/MAX DNS control\ndomains:\n- domain: remax.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: remax.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nobservations:\n- >-\n  No CAA records on either registrable domain, so any public CA may issue for\n  remax.com or remax.eu.\n- >-\n  No DNSSEC on either\
  \ domain.\n- >-\n  DMARC is enforced only at p=quarantine, not p=reject, on both domains.\n- >-\n  remax.com serves a DNS wildcard (CNAME customers.kvcore.com). The control probe\n  zzzznotreal.remax.com resolves identically to developer.remax.com,\n  developers.remax.com, docs.remax.com, status.remax.com and trust.remax.com -\n  none of those hostnames is a service RE/MAX runs. A wildcard that answers on\n  443 for every conceivable subdomain is itself a security-relevant posture\n  (subdomain-confusion and phishing surface).\n- >-\n  api.remax.com is a dangling CNAME to api.remax-prod.booj.io, which returns\n  NXDOMAIN - a classic subdomain-takeover shape left behind by the decommissioned\n  booj platform.\n- >-\n  The API and OAuth hosts negotiate TLS 1.2 and set no HSTS, while the two\n  Postman documentation hosts (which carry no data) are TLS 1.3 with HSTS\n  preload. The transport hardening is inverted relative to where the risk is.\nprograms:\n  security_txt: absent on every host\
  \ probed\n  vulnerability_disclosure: none published\n  trust_center: >-\n    none. trust.remax.com answers 403 only because of the remax.com wildcard; it\n    is not a trust center.\n  probe: 0-working/probe-security-programs.py returned vdp=none trust=none (2026-07-26)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/re-max/refs/heads/main/security/re-max-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real-Estate
- United States
- Brokerage
- Property Listings
- MLS
- RESO
- IDX
- PropTech
- Franchising
- Mortgage
- Rentals
---
