---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: suncorpgroup.com.au
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: suncorp.com.au
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vero.com.au
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aami.com.au
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gio.com.au
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: apia.com.au
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shannons.com.au
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bingle.com.au
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: terrischeer.com.au
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vero.co.nz
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aainsurance.co.nz
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: verocentral.com.au
  spf: true
hosts:
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: www.suncorpgroup.com.au
  hsts: false
  hsts_max_age: null
  https: true
  note: Corporate site. The ONLY host in the estate with no Strict-Transport-Security header. Fronted by an Imperva Incapsula WAF that answers scripted path requests with a challenge/noindex shell, so HTTP status codes from this host are not evidence of a real page.
  role: corporate
  tls_version: TLSv1.3
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: www.suncorp.com.au
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15768000
  https: true
  note: Post-divestment this host serves Suncorp Bank (sold to ANZ 31 July 2024) content alongside the Suncorp insurance brand; /security is a consumer online safety page, not a vulnerability disclosure policy.
  role: brand
  tls_version: TLSv1.3
- cert_expires: Nov 25 23:59:59 2026 GMT
  host: www.vero.com.au
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15768000
  https: true
  role: brand
  tls_version: TLSv1.3
- cert_expires: Nov 25 23:59:59 2026 GMT
  host: www.aami.com.au
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 31557600
  https: true
  role: brand
  tls_version: TLSv1.3
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: www.gio.com.au
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  role: brand
  tls_version: TLSv1.3
- cert_expires: Nov 25 23:59:59 2026 GMT
  host: www.apia.com.au
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15768000
  https: true
  role: brand
  tls_version: TLSv1.3
- cert_expires: Sep 21 23:59:59 2026 GMT
  host: www.shannons.com.au
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  role: brand
  tls_version: TLSv1.3
- cert_expires: Nov 25 23:59:59 2026 GMT
  host: www.bingle.com.au
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 31557600
  https: true
  note: developer.bingle.com.au and api.bingle.com.au remain as dangling CNAMEs to decommissioned AWS ap-southeast-2 load balancers; neither target resolves.
  role: brand
  tls_version: TLSv1.3
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: www.terrischeer.com.au
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 31557600
  https: true
  role: brand
  tls_version: TLSv1.3
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: www.vero.co.nz
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15768000
  https: true
  role: brand-nz
  tls_version: TLSv1.3
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: www.aainsurance.co.nz
  hsts: false
  hsts_max_age: null
  https: true
  note: Served from CloudFront and answers every path with HTTP 202 and an empty body (bot challenge), so status codes from this host are not evidence of a page.
  role: brand-nz
  tls_version: TLSv1.3
- cert_expires: Sep  3 23:59:59 2026 GMT
  host: online.verocentral.com.au
  hsts: false
  hsts_max_age: null
  https: true
  note: Identity provider behind the VeroEdge / Vero Intermediary Portal broker login (Apache Tomcat). No anonymous OIDC or OAuth discovery document is served.
  role: gated-idp
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Suncorp Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Suncorp Group, probed live across 12 host(s) and 12 registrable domain(s). 12 host(s) serve HTTPS (up to TLSv1.3); 9 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Suncorp Group
provider_slug: suncorp-group
slug: suncorp-group-domain-security
source_filename: suncorp-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: >-\n  Live DNS (dig DS/CAA/TXT), TLS (openssl s_client) and HTTP HEAD probes of every\n  Suncorp Group corporate, brand and gated-portal host reachable on 2026-07-25.\n  Extends the mechanical single-host probe to the full twelve-brand estate.\nnote: >-\n  Suncorp Group publishes no public API, so there is no API host to probe. The\n  hosts below are the corporate site, the Australian and New Zealand insurance\n  brand sites, and the gated broker identity-provider host. Absence of a record\n  (no DNSSEC, no CAA, no HSTS) is recorded as observed fact.\nhosts:\n- host: www.suncorpgroup.com.au\n  role: corporate\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: 'Jan 28 23:59:59 2027 GMT'\n  hsts: false\n  hsts_max_age: null\n  note: >-\n    Corporate site. The ONLY host in the estate with no Strict-Transport-Security\n    header. Fronted by an Imperva Incapsula WAF that answers scripted path\n    requests with a challenge/noindex\
  \ shell, so HTTP status codes from this host\n    are not evidence of a real page.\n- host: www.suncorp.com.au\n  role: brand\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: 'Dec  2 23:59:59 2026 GMT'\n  hsts: true\n  hsts_max_age: 15768000\n  hsts_include_subdomains: true\n  note: >-\n    Post-divestment this host serves Suncorp Bank (sold to ANZ 31 July 2024)\n    content alongside the Suncorp insurance brand; /security is a consumer online\n    safety page, not a vulnerability disclosure policy.\n- host: www.vero.com.au\n  role: brand\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: 'Nov 25 23:59:59 2026 GMT'\n  hsts: true\n  hsts_max_age: 15768000\n  hsts_include_subdomains: true\n- host: www.aami.com.au\n  role: brand\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: 'Nov 25 23:59:59 2026 GMT'\n  hsts: true\n  hsts_max_age: 31557600\n  hsts_include_subdomains: false\n- host: www.gio.com.au\n  role: brand\n  https: true\n  tls_version: TLSv1.3\n  cert_expires:\
  \ 'Nov 27 23:59:59 2026 GMT'\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: www.apia.com.au\n  role: brand\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: 'Nov 25 23:59:59 2026 GMT'\n  hsts: true\n  hsts_max_age: 15768000\n  hsts_include_subdomains: true\n- host: www.shannons.com.au\n  role: brand\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: 'Sep 21 23:59:59 2026 GMT'\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: www.bingle.com.au\n  role: brand\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: 'Nov 25 23:59:59 2026 GMT'\n  hsts: true\n  hsts_max_age: 31557600\n  hsts_include_subdomains: false\n  note: >-\n    developer.bingle.com.au and api.bingle.com.au remain as dangling CNAMEs to\n    decommissioned AWS ap-southeast-2 load balancers; neither target resolves.\n- host: www.terrischeer.com.au\n  role: brand\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: 'Dec  4 23:59:59 2026 GMT'\n\
  \  hsts: true\n  hsts_max_age: 31557600\n  hsts_include_subdomains: false\n- host: www.vero.co.nz\n  role: brand-nz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: 'Jan  7 23:59:59 2027 GMT'\n  hsts: true\n  hsts_max_age: 15768000\n  hsts_include_subdomains: true\n- host: www.aainsurance.co.nz\n  role: brand-nz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: 'Jan 27 23:59:59 2027 GMT'\n  hsts: false\n  hsts_max_age: null\n  note: >-\n    Served from CloudFront and answers every path with HTTP 202 and an empty body\n    (bot challenge), so status codes from this host are not evidence of a page.\n- host: online.verocentral.com.au\n  role: gated-idp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: 'Sep  3 23:59:59 2026 GMT'\n  hsts: false\n  hsts_max_age: null\n  note: >-\n    Identity provider behind the VeroEdge / Vero Intermediary Portal broker login\n    (Apache Tomcat). No anonymous OIDC or OAuth discovery document is served.\ndomains:\n- domain: suncorpgroup.com.au\n\
  \  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: suncorp.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: vero.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: aami.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: gio.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: apia.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: shannons.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: bingle.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: terrischeer.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: vero.co.nz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n \
  \ dmarc_policy: reject\n- domain: aainsurance.co.nz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: verocentral.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\nsummary:\n  hosts_probed: 12\n  domains_probed: 12\n  https_everywhere: true\n  tls13_everywhere: true\n  hsts_present: 9\n  hsts_absent: 3\n  hsts_absent_hosts:\n  - www.suncorpgroup.com.au\n  - www.aainsurance.co.nz\n  - online.verocentral.com.au\n  dnssec_signed: 0\n  caa_published: 0\n  spf_published: 12\n  dmarc_published: 12\n  dmarc_policy_reject: 12\n  reading: >-\n    Uniform and disciplined at the email layer — every one of the twelve\n    registrable domains publishes SPF and a DMARC policy of p=reject, which is\n    stronger than most of the Australian insurance cohort. Uniformly absent at the\n    DNS-integrity layer — zero DNSSEC signing and zero CAA records anywhere in the\n    estate. Transport is TLS 1.3 on every host, but HSTS is\
  \ missing on the\n    corporate domain and on the broker identity-provider host, which are the two\n    places it would matter most.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/suncorp-group/refs/heads/main/security/suncorp-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Australia
- Property and Casualty
- General Insurance
- Carrier
- Personal Lines
- Commercial Lines
- Claims
- Underwriting
- Broker
- Partner Gated
- New Zealand
---
