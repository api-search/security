---
description: ''
domains: []
hosts: []
kind: domain-security
layout: security
method: probed
name: Triblio Domain Security
name_suffix: Domain Security
overview: Domain security posture for Triblio, probed live across 0 host(s) and 0 registrable domain(s).
provider_name: Triblio
provider_slug: triblio
slug: triblio-domain-security
source_filename: triblio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  Direct DNS and TLS probes of triblio.com and its subdomains against 8.8.8.8\n  and against the domain's own delegated authoritative nameservers, plus a\n  registry WHOIS lookup.\nname: Triblio — domain security posture\nslug: triblio\n\nreachable: false\n\nsummary: >-\n  triblio.com cannot be assessed for TLS, HSTS, DNSSEC, CAA, SPF or DMARC\n  because the domain serves no DNS at all. The registration is alive and\n  defensively locked — MarkMonitor, expiring 2027-03-19, with clientDelete,\n  clientTransfer and clientUpdate prohibited — and the registry still delegates\n  the zone to four Amazon Route 53 nameservers. Those nameservers answer REFUSED\n  for triblio.com, which is what Route 53 returns when the hosted zone behind a\n  delegation has been deleted. The result is a registered, locked, brand-\n  protected domain with an empty delegation: no A, no MX, no TXT, no SOA. That\n  is the decisive evidence that the Triblio\
  \ web surface was decommissioned\n  rather than redirected.\n\nregistration:\n  registrar: MarkMonitor Inc.\n  created: '2013-03-19'\n  updated: '2026-02-15'\n  expires: '2027-03-19'\n  status:\n    - clientDeleteProhibited\n    - clientTransferProhibited\n    - clientUpdateProhibited\n  note: >-\n    Registrar and lock set are consistent with a corporate brand-protection\n    holding, which is how Foundry/IDG would park an absorbed brand.\n\ndelegation:\n  nameservers:\n    - ns-246.awsdns-30.com\n    - ns-515.awsdns-00.net\n    - ns-1356.awsdns-41.org\n    - ns-1562.awsdns-03.co.uk\n  authoritative_response: REFUSED\n  note: >-\n    Queried ns-246.awsdns-30.com directly for triblio.com A and SOA. Both\n    returned status REFUSED with zero answer and zero authority records — the\n    Route 53 hosted zone no longer exists.\n\nrecords:\n  a: []\n  mx: []\n  txt: []\n  soa: null\n  caa: null\n  dnssec: null\n\nchecks:\n  tls: not-assessable\n  hsts: not-assessable\n  dnssec: not-assessable\n\
  \  caa: not-assessable\n  spf: not-assessable\n  dmarc: not-assessable\n  note: >-\n    \"not-assessable\" is distinct from \"absent\". No connection can be opened to a\n    host that does not resolve, so recording these as failures would be a false\n    negative about the provider's security posture rather than a measurement.\n\nsubdomains_probed:\n  - host: www.triblio.com\n    resolves: false\n  - host: app.triblio.com\n    resolves: false\n  - host: api.triblio.com\n    resolves: false\n  - host: learning.triblio.com\n    resolves: false\n\nsuccessor_hosts:\n  - host: learning.foundryco.com\n    resolves: true\n    cname: triblio.zendesk.com\n    note: >-\n      The only surviving host that is unambiguously Triblio's own — the Zendesk\n      instance is still named \"triblio\". Fronted by Cloudflare, which returns\n      403 to every automated request.\n  - host: intent.foundryco.com\n    resolves: true\n    cname: intent-web-1606417831.us-east-1.elb.amazonaws.com\n    note: >-\n \
  \     Foundry Intent application. AWS ELB answers 503 on every path including\n      /login, across repeated probes.\n\nchecked: '2026-08-12'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/triblio/refs/heads/main/security/triblio-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Account Based Marketing
- Advertising
- Intent Data
- Marketing Technology
- MarTech
- B2B Marketing
- Sales Acceleration
- Web Personalization
- Audience Segmentation
- Demand Generation
- CRM Integration
- Foundry
- IDG
---
