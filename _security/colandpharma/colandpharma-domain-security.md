---
description: ''
domains:
- a_record: false
  authoritative_answer: Queried the authoritative nameserver directly; it returned no A record, confirming the zone carries no host content rather than a resolver-side failure.
  caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: colandpharma.com
  mx: false
  nameservers:
  - a6.share-dns.com
  - b6.share-dns.net
  registered: true
  spf: false
hosts:
- error: NXDOMAIN-equivalent (NOERROR, zero answers) — no A/AAAA record
  host: colandpharma.com
  http_status: null
  https: false
  resolves: false
- host: www.colandpharma.com
  http_status: null
  https: false
  resolves: false
- host: api.colandpharma.com
  http_status: null
  https: false
  resolves: false
- host: docs.colandpharma.com
  http_status: null
  https: false
  resolves: false
- host: developer.colandpharma.com
  http_status: null
  https: false
  resolves: false
kind: domain-security
layout: security
method: probed
name: Colandpharma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for colandpharma, probed live across 5 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: colandpharma
provider_slug: colandpharma
slug: colandpharma-domain-security
source_filename: colandpharma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/WHOIS/HTTP probes of the apis.yml Website host (colandpharma.com)\nsummary: >-\n  colandpharma.com is a registered but dormant domain. It delegates to nameservers\n  but publishes no A/AAAA, MX, TXT, SPF, DMARC or CAA records, so there is no\n  reachable website, mail surface or API surface to assess. All probe results below\n  are verified absences, not failures to probe.\nhosts:\n- host: colandpharma.com\n  https: false\n  resolves: false\n  http_status: null\n  error: NXDOMAIN-equivalent (NOERROR, zero answers) — no A/AAAA record\n- host: www.colandpharma.com\n  https: false\n  resolves: false\n  http_status: null\n- host: api.colandpharma.com\n  https: false\n  resolves: false\n  http_status: null\n- host: docs.colandpharma.com\n  https: false\n  resolves: false\n  http_status: null\n- host: developer.colandpharma.com\n  https: false\n  resolves: false\n  http_status: null\ndomains:\n- domain: colandpharma.com\n\
  \  registered: true\n  dnssec: false\n  a_record: false\n  mx: false\n  spf: false\n  dmarc: false\n  dmarc_policy: null\n  caa: []\n  nameservers:\n  - a6.share-dns.com\n  - b6.share-dns.net\n  authoritative_answer: >-\n    Queried the authoritative nameserver directly; it returned no A record, confirming\n    the zone carries no host content rather than a resolver-side failure.\nregistration:\n  registrar: Gname.com Pte. Ltd.\n  registrar_iana_id: 1923\n  registrar_whois: whois.gname.com\n  created: '2007-09-21'\n  updated: '2025-11-20'\n  expires: '2027-09-21'\n  status:\n  - clientTransferProhibited\n  dnssec: unsigned\n  source: whois.verisign-grs.com\nfindings:\n- id: no-web-presence\n  severity: info\n  detail: >-\n    No HTTP(S) endpoint exists on the apex or any probed subdomain, so TLS version,\n    certificate expiry and HSTS could not be evaluated.\n- id: no-mail-authentication\n  severity: info\n  detail: >-\n    No MX, SPF or DMARC records are published. The domain sends\
  \ and receives no mail\n    as configured.\n- id: dnssec-unsigned\n  severity: info\n  detail: The domain is not DNSSEC signed (confirmed by WHOIS and absent DS/DNSKEY records).\n- id: registration-current\n  severity: info\n  detail: >-\n    Registration is active and was renewed through 2027-09-21, so the domain is held\n    rather than abandoned — consistent with a parked or pre-launch holding.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/colandpharma/refs/heads/main/security/colandpharma-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Pharmaceuticals
- Health
- Venture Backed
- Dormant
---
