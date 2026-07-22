---
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: murmurcars.com
  mx: true
  mx_provider: Google Workspace
  note: Google Workspace mail is still configured (MX present) but no SPF, DMARC, CAA, or DNSSEC records are published.
  spf: false
  txt:
  - google-site-verification=VenwwoNIDt3-D5TjmucHV0We9RcWy8n3z0NhYhfPMmE
hosts:
- a_record: false
  host: murmurcars.com
  https: false
  note: apex has NS but no A record; no reachable HTTPS host
  reachable: false
- a_record: true
  host: blog.murmurcars.com
  https: false
  ip: 18.209.59.200
  note: resolves but connection refused on 443
  reachable: false
kind: domain-security
layout: security
method: probed
name: Murmur Technologies Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Murmur Technologies INC, probed live across 2 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Murmur Technologies INC
provider_slug: murmur-technologies-inc
slug: murmur-technologies-inc-domain-security
source_filename: murmur-technologies-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: dig DNS probe of murmurcars.com (apis.yml Website host); HTTPS unreachable\nnote: >-\n  The provider's web hosts do not resolve to a live server. The apex domains\n  murmurcars.com and murmurads.com carry NS records (AWS Route 53) but no A\n  record, and blog.murmurcars.com resolves to 18.209.59.200 but refuses HTTPS\n  connections. TLS/HSTS could not be probed because no host is reachable. Only\n  DNS-level records are recorded below; the operation appears dormant.\nhosts:\n  - host: murmurcars.com\n    https: false\n    reachable: false\n    a_record: false\n    note: apex has NS but no A record; no reachable HTTPS host\n  - host: blog.murmurcars.com\n    https: false\n    reachable: false\n    a_record: true\n    ip: 18.209.59.200\n    note: resolves but connection refused on 443\ndomains:\n  - domain: murmurcars.com\n    dnssec: false\n    caa: []\n    spf: false\n    dmarc: false\n    dmarc_policy: null\n    mx: true\n \
  \   mx_provider: Google Workspace\n    txt:\n      - google-site-verification=VenwwoNIDt3-D5TjmucHV0We9RcWy8n3z0NhYhfPMmE\n    note: >-\n      Google Workspace mail is still configured (MX present) but no SPF, DMARC,\n      CAA, or DNSSEC records are published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/murmur-technologies-inc/refs/heads/main/security/murmur-technologies-inc-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Advertising
- AdTech
- Out-of-Home Advertising
- Digital Billboards
- Mobile Advertising
- Marketing
---
