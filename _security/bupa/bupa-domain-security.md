---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bupa.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bupa.com.au
  spf: true
- caa:
  - 0 issue "pki.goog"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bupa.cl
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bupa.co.uk
  spf: true
hosts:
- cert_expires: Dec 12 13:51:15 2026 GMT
  host: www.bupa.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: portal.api.bupa.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: api.bupa.com.au
  hsts: null
  https: true
  note: Imperva-fronted APIM gateway; returns HTTP 502 to anonymous callers, so no HSTS header is observable from an unauthenticated request.
  tls_version: TLSv1.3
- cert_expires: Jan 28 14:56:29 2027 GMT
  host: apidoc.bupa.cl
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 28 14:56:29 2027 GMT
  host: api.bupa.cl
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  6 09:47:07 2027 GMT
  host: www.bupa.co.uk
  hsts: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bupa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bupa, probed live across 6 host(s) and 4 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 5 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bupa
provider_slug: bupa
slug: bupa-domain-security
source_filename: bupa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + market-unit API hosts\nnote: >-\n  Probed with 0-working/probe-domain-security.py for the group and Bupa\n  Australia hosts, then extended by hand for the Bupa Chile and Bupa UK market\n  units (openssl s_client for TLS, curl -I for HSTS, dig for CAA/SPF/DMARC/\n  DNSKEY), which the script does not reach from a baseURL walk. Absence of a\n  record is recorded as absence, not as an error.\nhosts:\n- host: www.bupa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 13:51:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: portal.api.bupa.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.bupa.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: null\n  note: >-\n    Imperva-fronted APIM gateway; returns HTTP 502 to anonymous callers,\
  \ so no\n    HSTS header is observable from an unauthenticated request.\n- host: apidoc.bupa.cl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 14:56:29 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n  hsts_include_subdomains: true\n- host: api.bupa.cl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 14:56:29 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n  hsts_include_subdomains: true\n- host: www.bupa.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 09:47:07 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_preload: true\ndomains:\n- domain: bupa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: bupa.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: bupa.cl\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: bupa.co.uk\n  dnssec: false\n\
  \  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\nsummary:\n  hosts_probed: 6\n  https_everywhere: true\n  tls13_everywhere: true\n  hsts_hosts: 5\n  domains_probed: 4\n  dnssec_domains: 0\n  caa_domains: 1\n  spf_domains: 4\n  dmarc_reject_domains: 4\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bupa/refs/heads/main/security/bupa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- United Kingdom
- Health Insurance
- Life and Health
- Carrier
- Healthcare
- Aged Care
- Claims
- Policy Administration
- Partner Gated
---
