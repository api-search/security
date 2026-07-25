---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bluecross.ca
  nameservers:
  - dns1.cidc.telus.com
  - dns2.cidc.telus.com
  note: DMARC is published but at p=none (monitor only), so no enforcement against spoofed mail from the brand domain. No CAA records, so certificate issuance is unconstrained. No DNSSEC.
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: medaviebc.ca
  nameservers:
  - simon.ns.cloudflare.com
  - kia.ns.cloudflare.com
  note: SPF and DMARC are delegated to Proofpoint (pphosted.com); DMARC is also p=none. No CAA, no DNSSEC.
  spf: true
hosts:
- cert_expires: Oct 17 16:18:54 2026 GMT
  host: www.bluecross.ca
  hsts: true
  hsts_max_age: 300
  https: true
  note: HSTS max-age of 300 seconds is far below the 31536000 the member plans use and below any preload threshold — effectively a token policy on the national brand site.
  plan: Canadian Association of Blue Cross Plans
  tls_version: TLSv1.3
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: pac.bluecross.ca
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  plan: Pacific Blue Cross
  tls_version: TLSv1.3
- cert_expires: Oct 23 08:03:30 2026 GMT
  host: ab.bluecross.ca
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Cloudflare bot management returns 403/interstitial to non-browser clients.
  plan: Alberta Blue Cross
  tls_version: TLSv1.3
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: on.bluecross.ca
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  plan: Ontario / Quebec Blue Cross (Canassurance)
  tls_version: TLSv1.3
- cert_expires: Oct  9 05:45:50 2026 GMT
  host: www.medaviebc.ca
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  plan: Medavie Blue Cross
  tls_version: TLSv1.3
- cert_expires: Oct 19 19:17:31 2026 GMT
  host: www.sk.bluecross.ca
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15552000
  https: true
  plan: Saskatchewan Blue Cross
  tls_version: TLSv1.3
- cert_expires: Jan 25 23:59:59 2027 GMT
  host: www.mb.bluecross.ca
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 31536000
  https: true
  plan: Manitoba Blue Cross
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Canadian Blue Cross Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blue Cross Canada, probed live across 7 host(s) and 2 registrable domain(s). 7 host(s) serve HTTPS (up to TLSv1.3); 7 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Blue Cross Canada
provider_slug: canadian-blue-cross
slug: canadian-blue-cross-domain-security
source_filename: canadian-blue-cross-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: >-\n  live DNS/TLS/HTTP probes of the apis.yml hosts (0-working/probe-domain-security.py) extended\n  by hand to every operating Blue Cross member-plan host in the federation\nhosts:\n- host: www.bluecross.ca\n  plan: Canadian Association of Blue Cross Plans\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 16:18:54 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n  note: >-\n    HSTS max-age of 300 seconds is far below the 31536000 the member plans use and below any\n    preload threshold — effectively a token policy on the national brand site.\n- host: pac.bluecross.ca\n  plan: Pacific Blue Cross\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: ab.bluecross.ca\n  plan: Alberta Blue Cross\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 08:03:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n\
  \  hsts_include_subdomains: true\n  note: Cloudflare bot management returns 403/interstitial to non-browser clients.\n- host: on.bluecross.ca\n  plan: Ontario / Quebec Blue Cross (Canassurance)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: www.medaviebc.ca\n  plan: Medavie Blue Cross\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 05:45:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: www.sk.bluecross.ca\n  plan: Saskatchewan Blue Cross\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 19:17:31 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n  hsts_include_subdomains: true\n- host: www.mb.bluecross.ca\n  plan: Manitoba Blue Cross\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: false\ndomains:\n- domain:\
  \ bluecross.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  nameservers: [dns1.cidc.telus.com, dns2.cidc.telus.com]\n  note: >-\n    DMARC is published but at p=none (monitor only), so no enforcement against spoofed mail from\n    the brand domain. No CAA records, so certificate issuance is unconstrained. No DNSSEC.\n- domain: medaviebc.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  nameservers: [simon.ns.cloudflare.com, kia.ns.cloudflare.com]\n  note: >-\n    SPF and DMARC are delegated to Proofpoint (pphosted.com); DMARC is also p=none. No CAA, no\n    DNSSEC.\nsummary:\n  https_everywhere: true\n  tls13_everywhere: true\n  hsts_hosts: 7\n  dnssec_domains: 0\n  caa_domains: 0\n  dmarc_enforcing_domains: 0\n  note: >-\n    Transport hygiene is uniformly good across the federation; domain-level controls (DNSSEC,\n    CAA, DMARC enforcement) are uniformly absent.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canadian-blue-cross/refs/heads/main/security/canadian-blue-cross-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Canada
- Health Insurance
- Dental Benefits
- Travel Insurance
- Life Insurance
- Employee Benefits
- Group Benefits
- Claims
- Carrier
- Association
- No Public API
---
