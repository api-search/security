---
description: ''
domains: []
hosts:
- error: NOERROR with no A/AAAA answer — the apex publishes no address record, so no TLS connection is possible.
  host: microbyre.com
  hsts: null
  https: false
  resolves: false
  tls_version: null
- cname: dw7qr6qh3v5bt.cloudfront.net
  error: Dangling CNAME — the CloudFront distribution dw7qr6qh3v5bt.cloudfront.net returns NOERROR with no answer, i.e. the distribution has been deleted or disabled.
  host: www.microbyre.com
  hsts: null
  https: false
  resolves: false
  tls_version: null
kind: domain-security
layout: security
method: probed
name: Microbyre Domain Security
name_suffix: Domain Security
overview: Domain security posture for MicroByre, probed live across 2 host(s) and 0 registrable domain(s).
provider_name: MicroByre
provider_slug: microbyre
slug: microbyre-domain-security
source_filename: microbyre-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: dig @8.8.8.8 + TLS connect attempts against microbyre.com, 2026-08-25\nnote: >-\n  MicroByre is out of business and its web surface is gone, but the registration is\n  still held and still carries live mail DNS. Recorded because the DNS answers are\n  real observations; no DomainSecurity pointer is wired into apis.yml, because there\n  is no served host for that pointer to assert.\nhosts:\n  - host: microbyre.com\n    https: false\n    resolves: false\n    tls_version: null\n    hsts: null\n    error: >-\n      NOERROR with no A/AAAA answer — the apex publishes no address record, so no\n      TLS connection is possible.\n  - host: www.microbyre.com\n    https: false\n    resolves: false\n    cname: dw7qr6qh3v5bt.cloudfront.net\n    tls_version: null\n    hsts: null\n    error: >-\n      Dangling CNAME — the CloudFront distribution dw7qr6qh3v5bt.cloudfront.net\n      returns NOERROR with no answer, i.e. the distribution has been\
  \ deleted or\n      disabled.\ndns:\n  registrable_domain: microbyre.com\n  nameservers:\n    - dns1.registrar-servers.com\n    - dns2.registrar-servers.com\n  dnssec: false\n  dnssec_evidence: no DNSKEY records returned\n  caa: []\n  caa_present: false\n  spf: 'v=spf1 include:_spf.protonmail.ch ~all'\n  spf_present: true\n  dmarc: 'v=DMARC1; p=quarantine'\n  dmarc_present: true\n  dmarc_policy: quarantine\n  mx:\n    - 10 mail.protonmail.ch\n    - 20 mailsec.protonmail.ch\n  txt_other:\n    - protonmail-verification=946871cde9fd1855f8033a5733f3531f2a894966\nfindings:\n  - The company website is unreachable; DNS resolves no address for the apex or www.\n  - Mail is still delivered (Proton Mail MX, SPF and DMARC quarantine present).\n  - No DNSSEC and no CAA records are published.\n  - >-\n    www.microbyre.com is a dangling CNAME at a deleted CloudFront distribution — a\n    subdomain-takeover shape worth flagging to whoever still holds the registration.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microbyre/refs/heads/main/security/microbyre-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Biotechnology
- Synthetic Biology
- Industrial Biotechnology
- Bioengineering
- Climate Tech
- Chemicals
---
