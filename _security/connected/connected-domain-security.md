---
description: ''
domains:
- caa: []
  created: '2010-03-08'
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: connectedhq.com
  nameservers:
  - dns1.p09.nsone.net
  - dns2.p09.nsone.net
  - dns3.p09.nsone.net
  - dns4.p09.nsone.net
  - ns1-42.azure-dns.com
  - ns2-42.azure-dns.net
  - ns3-42.azure-dns.org
  - ns4-42.azure-dns.info
  null_mx: true
  registrar: MarkMonitor Inc.
  registry_expiry: '2027-03-08'
  spf: true
hosts:
- host: connectedhq.com
  http_status: null
  https: false
  note: DNS resolution failed (no A/CNAME record); host serves no site.
  resolves: false
kind: domain-security
layout: security
method: probed
name: Connected Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Connected, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Connected
provider_slug: connected
slug: connected-domain-security
source_filename: connected-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts (no OpenAPI in repo)\nnote: connectedhq.com publishes no A or CNAME record and serves no content, so no TLS/HSTS\n  posture can be observed. The zone is still actively managed (SPF, DMARC p=reject, RFC 7505\n  null MX) which is consistent with a domain held defensively by the acquirer rather than\n  abandoned. See apis.yml x-domain-note.\nhosts:\n- host: connectedhq.com\n  https: false\n  resolves: false\n  http_status: null\n  note: DNS resolution failed (no A/CNAME record); host serves no site.\ndomains:\n- domain: connectedhq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  null_mx: true\n  registrar: MarkMonitor Inc.\n  created: '2010-03-08'\n  registry_expiry: '2027-03-08'\n  nameservers:\n  - dns1.p09.nsone.net\n  - dns2.p09.nsone.net\n  - dns3.p09.nsone.net\n  - dns4.p09.nsone.net\n  - ns1-42.azure-dns.com\n  - ns2-42.azure-dns.net\n  - ns3-42.azure-dns.org\n\
  \  - ns4-42.azure-dns.info\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/connected/refs/heads/main/security/connected-domain-security.yml
summary_line: DMARC
tags:
- Company
- Defunct
- Acquired
- CRM
- Contacts
- Address Book
- Relationship Management
- Social
---
