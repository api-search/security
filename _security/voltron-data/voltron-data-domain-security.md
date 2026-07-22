---
description: ''
domains:
- caa: null
  delegation: lame (authoritative servers REFUSED all queries at probe time)
  dmarc: null
  dnssec: null
  domain: voltrondata.com
  expiry: '2026-10-18'
  nameservers:
  - ns-368.awsdns-46.com
  - ns-761.awsdns-31.net
  - ns-1358.awsdns-41.org
  - ns-1934.awsdns-49.co.uk
  record_note: DNSSEC/CAA/SPF/DMARC unprobeable — the entire zone returns REFUSED, so no records of any type are served
  registered: true
  registrar: Amazon Registrar, Inc.
  spf: null
hosts:
- error: DNS SERVFAIL — delegated nameservers (ns-368.awsdns-46.com et al.) return REFUSED (lame delegation)
  host: voltrondata.com
  https: false
  resolves: false
- error: DNS SERVFAIL — same lame-delegated zone
  host: www.voltrondata.com
  https: false
  resolves: false
kind: domain-security
layout: security
method: probed
name: Voltron Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Voltron Data, probed live across 2 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Voltron Data
provider_slug: voltron-data
slug: voltron-data-domain-security
source_filename: voltron-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: dig (8.8.8.8 + authoritative), DNS-over-HTTPS (dns.google, cloudflare-dns.com), whois, curl\nnote: >-\n  voltrondata.com is registered and ACTIVE (Amazon Registrar, expiry 2026-10-18,\n  delegated to awsdns nameservers) but the Route 53 hosted zone behind the\n  delegation no longer answers: all four delegated nameservers return REFUSED\n  for every query (lame delegation), so the domain fails to resolve globally\n  (SERVFAIL at Google and Cloudflare public resolvers). The website, docs, and\n  any subdomains are unreachable as of this probe. The last successful Wayback\n  Machine capture of https://voltrondata.com/ was 2026-02-13 (HTTP 200).\nhosts:\n  - host: voltrondata.com\n    resolves: false\n    https: false\n    error: 'DNS SERVFAIL — delegated nameservers (ns-368.awsdns-46.com et al.) return REFUSED (lame delegation)'\n  - host: www.voltrondata.com\n    resolves: false\n    https: false\n    error: 'DNS SERVFAIL — same\
  \ lame-delegated zone'\ndomains:\n  - domain: voltrondata.com\n    registered: true\n    registrar: Amazon Registrar, Inc.\n    expiry: '2026-10-18'\n    nameservers:\n      - ns-368.awsdns-46.com\n      - ns-761.awsdns-31.net\n      - ns-1358.awsdns-41.org\n      - ns-1934.awsdns-49.co.uk\n    delegation: lame (authoritative servers REFUSED all queries at probe time)\n    dnssec: null\n    caa: null\n    spf: null\n    dmarc: null\n    record_note: 'DNSSEC/CAA/SPF/DMARC unprobeable — the entire zone returns REFUSED, so no records of any type are served'\nevidence:\n  - kind: doh\n    source: https://dns.google/resolve?name=voltrondata.com&type=A\n    result: 'Status 2 (SERVFAIL): \"Name servers refused query (lame delegation?)\" — all four awsdns hosts rcode=REFUSED'\n  - kind: doh\n    source: https://cloudflare-dns.com/dns-query?name=voltrondata.com&type=A\n    result: 'Status 2 (SERVFAIL): EDE 22 \"No Reachable Authority at delegation voltrondata.com\", EDE 23 REFUSED'\n  - kind: whois\n\
  \    source: whois voltrondata.com\n    result: 'ACTIVE, Amazon Registrar, Registry Expiry 2026-10-18, clientTransferProhibited, awsdns nameservers'\n  - kind: wayback\n    source: http://archive.org/wayback/available?url=voltrondata.com&timestamp=20260721\n    result: 'closest snapshot 2026-02-13 (status 200) — site was live in mid-February 2026'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voltron-data/refs/heads/main/security/voltron-data-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Data
- Analytics
- GPU
- SQL
- Query Engines
- Apache Arrow
- Open Source
---
