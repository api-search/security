---
description: ''
domains:
- caa: []
  dmarc: none
  dnssec_detail: DS at .tech references a DNSKEY that is not published in the zone; validating resolvers SERVFAIL
  dnssec_dnskey_in_zone: false
  dnssec_ds_at_parent: true
  dnssec_status: broken
  domain: thistle.tech
  mx: []
  nameservers:
  - ns1.dreamhost.com
  - ns2.dreamhost.com
  - ns3.dreamhost.com
  spf: false
hosts:
- a_record: none
  aaaa_record: none
  host: thistle.tech
  https: unknown
  resolves: false
  resolves_reason: dnssec-servfail (DS present, no DNSKEY in zone)
- host: www.thistle.tech
  https: unknown
  resolves: false
  resolves_reason: nxdomain
kind: domain-security
layout: security
method: probed
name: Thistle Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Thistle Technologies, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present.'
provider_name: Thistle Technologies
provider_slug: thistle-technologies
slug: thistle-technologies-domain-security
source_filename: thistle-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: https://dns.google/resolve (DoH, DNSSEC-validating + CD=1 bypass)\nnotes: >-\n  thistle.tech is the company's canonical domain but currently fails DNSSEC\n  validation: the .tech parent zone publishes a DS record (keytag 1792, alg 8,\n  digest type 2) for thistle.tech, yet the zone itself publishes NO matching\n  DNSKEY, so every validating resolver returns SERVFAIL and the name does not\n  resolve (curl/WebFetch see ENOTFOUND). With DNSSEC checking disabled (CD=1)\n  the apex has no A/AAAA record (NODATA) and www / api / docs / developer / app /\n  blog / portal subdomains are NXDOMAIN, so no web host is currently served. No\n  MX and no TXT (no SPF) are published at the apex. Nameservers are DreamHost.\n  Absence of records here is recorded, not inferred.\nhosts:\n  - host: thistle.tech\n    resolves: false\n    resolves_reason: dnssec-servfail (DS present, no DNSKEY in zone)\n    a_record: none\n    aaaa_record: none\n   \
  \ https: unknown\n  - host: www.thistle.tech\n    resolves: false\n    resolves_reason: nxdomain\n    https: unknown\ndomains:\n  - domain: thistle.tech\n    nameservers: [ns1.dreamhost.com, ns2.dreamhost.com, ns3.dreamhost.com]\n    dnssec_ds_at_parent: true\n    dnssec_dnskey_in_zone: false\n    dnssec_status: broken\n    dnssec_detail: DS at .tech references a DNSKEY that is not published in the zone; validating resolvers SERVFAIL\n    caa: []\n    spf: false\n    dmarc: none\n    mx: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thistle-technologies/refs/heads/main/security/thistle-technologies-domain-security.yml
summary_line: DMARC
tags:
- Company
- Device Security
- Embedded Security
- IoT Security
- Firmware Updates
- Over-the-Air Updates
- Secure Boot
- Edge AI
- Security
---
