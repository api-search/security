---
description: ''
domains:
- a_records: []
  aaaa_records: []
  assessment: The zone is alive but web-dead. Mail is still routed to Google Workspace with a strict SPF (-all) and DMARC monitoring via EasyDMARC, which is consistent with a wind-down estate retaining the domain for correspondence. No CAA is published and the zone is unsigned (no DS/DNSKEY). There is no web host, so no HTTP surface exists to secure.
  caa: []
  dmarc: true
  dmarc_policy: none
  dmarc_record: v=DMARC1;p=none;rua=mailto:system@vesttoo.com,mailto:8f830c3efa@rua.easydmarc.us;ruf=mailto:8f830c3efa@ruf.easydmarc.us;fo=1;
  dns_rcode: NOERROR
  dns_zone_present: true
  dnssec: false
  domain: vesttoo.com
  mx:
  - aspmx.l.google.com
  - alt1.aspmx.l.google.com
  - alt2.aspmx.l.google.com
  mx_present: true
  nameservers:
  - ns11.domaincontrol.com
  - ns12.domaincontrol.com
  soa: ns11.domaincontrol.com. dns.jomax.net. 2025040378
  spf: true
  spf_record: v=spf1 include:_spf.google.com -all
hosts:
- cert_expires: null
  host: vesttoo.com
  hsts: null
  http_status: 0
  https: false
  note: No A, AAAA or CNAME record is published, so there is no web listener to negotiate TLS with. Every HTTPS request fails at connection setup (curl exit / status 000), not with an HTTP error code. TLS, HSTS and certificate fields are therefore not applicable rather than absent-by-choice.
  tls_version: null
- cert_expires: null
  host: www.vesttoo.com
  hsts: null
  http_status: 0
  https: false
  note: No A/AAAA record; same connection-level failure as the apex.
  tls_version: null
kind: domain-security
layout: security
method: probed
name: Vesttoo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vesttoo, probed live across 2 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Vesttoo
provider_slug: vesttoo
slug: vesttoo-domain-security
source_filename: vesttoo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of vesttoo.com (dig @8.8.8.8, curl)\nnote: >-\n  Rewritten 2026-09-02. The prior revision of this file profiled forgeglobal.com — a\n  third-party secondary-market venue that merely lists Vesttoo stock — because the only\n  Website pointer in apis.yml was that venue listing. Those numbers described Forge\n  Global's security posture, not Vesttoo's, and were removed. This file now probes\n  vesttoo.com, the company's own registered domain.\nhosts:\n- host: vesttoo.com\n  https: false\n  http_status: 000\n  tls_version: null\n  cert_expires: null\n  hsts: null\n  note: >-\n    No A, AAAA or CNAME record is published, so there is no web listener to negotiate TLS\n    with. Every HTTPS request fails at connection setup (curl exit / status 000), not with\n    an HTTP error code. TLS, HSTS and certificate fields are therefore not applicable\n    rather than absent-by-choice.\n- host: www.vesttoo.com\n  https:\
  \ false\n  http_status: 000\n  tls_version: null\n  cert_expires: null\n  hsts: null\n  note: No A/AAAA record; same connection-level failure as the apex.\ndomains:\n- domain: vesttoo.com\n  dns_zone_present: true\n  dns_rcode: NOERROR\n  soa: ns11.domaincontrol.com. dns.jomax.net. 2025040378\n  nameservers:\n  - ns11.domaincontrol.com\n  - ns12.domaincontrol.com\n  a_records: []\n  aaaa_records: []\n  mx_present: true\n  mx:\n  - aspmx.l.google.com\n  - alt1.aspmx.l.google.com\n  - alt2.aspmx.l.google.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com -all\n  dmarc: true\n  dmarc_policy: none\n  dmarc_record: v=DMARC1;p=none;rua=mailto:system@vesttoo.com,mailto:8f830c3efa@rua.easydmarc.us;ruf=mailto:8f830c3efa@ruf.easydmarc.us;fo=1;\n  assessment: >-\n    The zone is alive but web-dead. Mail is still routed to Google Workspace with a strict\n    SPF (-all) and DMARC monitoring via EasyDMARC, which is consistent with a wind-down\n    estate retaining\
  \ the domain for correspondence. No CAA is published and the zone is\n    unsigned (no DS/DNSKEY). There is no web host, so no HTTP surface exists to secure.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vesttoo/refs/heads/main/security/vesttoo-domain-security.yml
summary_line: DMARC
tags:
- Company
- Insurance
- Insurtech
- Reinsurance
- Insurance-Linked Securities
- Alternative Risk Transfer
- Capital Markets
- Financial Services
- Defunct
---
