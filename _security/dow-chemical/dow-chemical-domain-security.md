---
description: ''
domains:
- caa: []
  caa_note: No CAA record is published, so any CA may issue for dow.com.
  dmarc: true
  dmarc_note: p=quarantine with an aggregate reporting address, but no p=reject and no ruf.
  dmarc_policy: quarantine
  dmarc_record: v=DMARC1; p=quarantine; rua=mailto:fglsmtp@dow.com
  dnssec: false
  domain: dow.com
  spf: true
hosts:
- cert_expires: Mar 19 23:59:59 2027 GMT
  cert_issuer: DigiCert Global G3 TLS ECC SHA384 2020 CA1
  cert_subject: CN=*.dow.com, O=Dow Inc., L=Midland, ST=Michigan, C=US
  content_security_policy: null
  edge: akamai
  host: www.dow.com
  hsts: max-age=15768000 ; includeSubDomains
  hsts_include_subdomains: true
  hsts_max_age: 15768000
  hsts_preload: false
  https: true
  referrer_policy: strict-origin-when-cross-origin
  tls_version: TLSv1.3
  x_content_type_options: nosniff
  x_frame_options: SAMEORIGIN
- cert_expires: Mar 19 23:59:59 2027 GMT
  cert_subject: CN=*.dow.com, O=Dow Inc., L=Midland, ST=Michigan, C=US
  edge: akamai
  host: legal.dow.com
  hsts: max-age=15768000 ; includeSubDomains
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 19 23:59:59 2027 GMT
  cert_subject: CN=*.dow.com, O=Dow Inc., L=Midland, ST=Michigan, C=US
  edge: akamai
  host: corporate.dow.com
  hsts: max-age=15768000 ; includeSubDomains
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Dow Chemical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dow Inc. (formerly The Dow Chemical Company), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dow Inc. (formerly The Dow Chemical Company)
provider_slug: dow-chemical
slug: dow-chemical-domain-security
source_filename: dow-chemical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: >-\n  Live DNS/TLS/HTTP probes of every host this record knows: the Website host\n  (www.dow.com), the registrable domain, the legal host named in the dow.com footer, and\n  the corporate newsroom host. Dow publishes no API baseURL and no OpenAPI, so there are\n  no servers[] hosts to probe.\nnote: >-\n  All three subject hosts are one wildcard certificate (CN=*.dow.com, O=Dow Inc.,\n  Midland, Michigan) behind Akamai. HSTS IS served — a previous automated pass recorded\n  hsts: null because the Akamai edge answers a bare crawler User-Agent with a 403\n  interstitial; the header is present on that response and on the origin response alike.\nhosts:\n  - host: www.dow.com\n    https: true\n    tls_version: TLSv1.3\n    cert_issuer: DigiCert Global G3 TLS ECC SHA384 2020 CA1\n    cert_subject: CN=*.dow.com, O=Dow Inc., L=Midland, ST=Michigan, C=US\n    cert_expires: Mar 19 23:59:59 2027 GMT\n    hsts: max-age=15768000 ; includeSubDomains\n\
  \    hsts_max_age: 15768000\n    hsts_include_subdomains: true\n    hsts_preload: false\n    x_content_type_options: nosniff\n    x_frame_options: SAMEORIGIN\n    referrer_policy: strict-origin-when-cross-origin\n    content_security_policy: null\n    edge: akamai\n  - host: legal.dow.com\n    https: true\n    tls_version: TLSv1.3\n    cert_subject: CN=*.dow.com, O=Dow Inc., L=Midland, ST=Michigan, C=US\n    cert_expires: Mar 19 23:59:59 2027 GMT\n    hsts: max-age=15768000 ; includeSubDomains\n    edge: akamai\n  - host: corporate.dow.com\n    https: true\n    tls_version: TLSv1.3\n    cert_subject: CN=*.dow.com, O=Dow Inc., L=Midland, ST=Michigan, C=US\n    cert_expires: Mar 19 23:59:59 2027 GMT\n    hsts: max-age=15768000 ; includeSubDomains\n    edge: akamai\ndomains:\n  - domain: dow.com\n    dnssec: false\n    caa: []\n    caa_note: No CAA record is published, so any CA may issue for dow.com.\n    spf: true\n    dmarc: true\n    dmarc_policy: quarantine\n    dmarc_record: 'v=DMARC1;\
  \ p=quarantine; rua=mailto:fglsmtp@dow.com'\n    dmarc_note: >-\n      p=quarantine with an aggregate reporting address, but no p=reject and no ruf.\nfindings:\n  - HSTS is served on every host, includeSubDomains, ~182 days, not preloaded.\n  - No CAA record — an absence, and valid data, not an error.\n  - DNSSEC is not enabled on dow.com.\n  - DMARC is enforced at quarantine rather than reject.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dow-chemical/refs/heads/main/security/dow-chemical-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Materials Science
- Chemicals
- Manufacturing
- Fortune 500
- Specialty Chemicals
- Packaging
- Coatings
---
