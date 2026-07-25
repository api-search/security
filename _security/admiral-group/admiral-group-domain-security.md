---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: admiralgroup.co.uk
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: admiral.com
  spf: true
- caa:
  - 0 issue "amazon.com"
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
  dnssec: false
  domain: confused.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: veygo.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: admiralpioneer.com
  spf: true
hosts:
- cert_expires: Sep  8 07:58:48 2026 GMT
  host: www.admiralgroup.co.uk
  hsts: null
  https: true
  note: Bot-protected; HTTP requests from non-browser clients time out.
  tls_version: TLSv1.3
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: www.admiral.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: api.admiral.com
  hsts: null
  https: true
  note: Undocumented private backend; all paths return HTTP 502.
  tls_version: TLSv1.3
- cert_expires: Sep  1 12:09:59 2026 GMT
  host: www.confused.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 12:09:59 2026 GMT
  host: api.confused.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  note: Live private JSON gateway - returns {"statusCode":404,"message":"Resource not found"} on every probed path. No public spec, docs, or GraphQL surface.
  tls_version: TLSv1.3
- cert_expires: Oct 14 18:24:25 2026 GMT
  host: www.veygo.com
  hsts: null
  https: true
  note: Returns 403 to automated clients on every path.
  tls_version: TLSv1.3
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: api.veygo.com
  hsts: null
  https: true
  note: Private AWS API Gateway; 403 {"message":"Forbidden"} to anonymous callers.
  tls_version: TLSv1.3
- cert_expires: Sep 19 08:13:03 2026 GMT
  host: www.admiralpioneer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Admiral Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Admiral Group, probed live across 8 host(s) and 5 registrable domain(s). 8 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Admiral Group
provider_slug: admiral-group
slug: admiral-group-domain-security
source_filename: admiral-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + brand hosts\nnote: >-\n  Probed across every Admiral Group brand host that resolves, including the two\n  undocumented private API backends (api.admiral.com, api.veygo.com) and the\n  Confused.com private JSON gateway (api.confused.com). No Admiral Group\n  registrable domain signs with DNSSEC; only confused.com publishes CAA records.\n  Every domain publishes SPF and DMARC - admiralgroup.co.uk and admiral.com at\n  p=reject, the Pioneer-era brands (confused.com, veygo.com, admiralpioneer.com)\n  at p=quarantine.\nhosts:\n- host: www.admiralgroup.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 07:58:48 2026 GMT\n  hsts: null\n  note: Bot-protected; HTTP requests from non-browser clients time out.\n- host: www.admiral.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.admiral.com\n\
  \  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: null\n  note: Undocumented private backend; all paths return HTTP 502.\n- host: www.confused.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 12:09:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.confused.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 12:09:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  note: >-\n    Live private JSON gateway - returns {\"statusCode\":404,\"message\":\"Resource not\n    found\"} on every probed path. No public spec, docs, or GraphQL surface.\n- host: www.veygo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 18:24:25 2026 GMT\n  hsts: null\n  note: Returns 403 to automated clients on every path.\n- host: api.veygo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: null\n  note: Private AWS\
  \ API Gateway; 403 {\"message\":\"Forbidden\"} to anonymous callers.\n- host: www.admiralpioneer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 08:13:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: admiralgroup.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: admiral.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: confused.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain:\
  \ veygo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: admiralpioneer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nsummary:\n  hosts_probed: 9\n  domains_probed: 5\n  https_all: true\n  hsts_hosts: 4\n  dnssec_domains: 0\n  caa_domains: 1\n  spf_domains: 5\n  dmarc_domains: 5\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/admiral-group/refs/heads/main/security/admiral-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- United Kingdom
- Property and Casualty
- Motor Insurance
- Home Insurance
- Pet Insurance
- Travel Insurance
- Carrier
- Personal Lines
- Price Comparison
- Embedded Insurance
- Consumer Lending
- Underwriting
- Claims
- Company
---
