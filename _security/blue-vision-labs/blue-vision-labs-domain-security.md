---
description: DNS and transport-security posture for bluevisionlabs.com. The domain is still registered and still carries Google Workspace mail records, but it publishes no A/AAAA record, so there is no reachable web or API surface. Probed values below are recorded verbatim; absence of a record is real data, not a gap in probing.
domains:
- dns:
    a: []
    aaaa: []
    caa: []
    dmarc: null
    dnssec: false
    ds_records: []
    mx:
    - 1 aspmx.l.google.com.
    - 5 alt1.aspmx.l.google.com.
    - 5 alt2.aspmx.l.google.com.
    - 10 alt3.aspmx.l.google.com.
    - 10 alt4.aspmx.l.google.com.
    ns_present: true
    spf: v=spf1 include:_spf.google.com ~all
  domain: bluevisionlabs.com
  hsts:
    probed: false
    reason: host does not resolve
  http_status: null
  https_reachable: false
  nameservers:
  - ns-153.awsdns-19.com.
  - ns-568.awsdns-07.net.
  - ns-1396.awsdns-46.org.
  - ns-1562.awsdns-03.co.uk.
  notes: No A or AAAA record. curl to https://bluevisionlabs.com/ and https://www.bluevisionlabs.com/ both fail to connect (exit before HTTP).
  resolves: false
  tls:
    probed: false
    reason: host does not resolve
hosts: []
kind: domain-security
layout: security
method: probed
name: Blue Vision Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blue Vision Labs, probed live across 0 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Blue Vision Labs
provider_slug: blue-vision-labs
slug: blue-vision-labs-domain-security
source_filename: blue-vision-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: dig + curl probe of bluevisionlabs.com on 2026-07-20\nname: Blue Vision Labs Domain Security\ndescription: >-\n  DNS and transport-security posture for bluevisionlabs.com. The domain is still\n  registered and still carries Google Workspace mail records, but it publishes no\n  A/AAAA record, so there is no reachable web or API surface. Probed values below\n  are recorded verbatim; absence of a record is real data, not a gap in probing.\ndomains:\n- domain: bluevisionlabs.com\n  resolves: false\n  https_reachable: false\n  http_status: null\n  notes: >-\n    No A or AAAA record. curl to https://bluevisionlabs.com/ and\n    https://www.bluevisionlabs.com/ both fail to connect (exit before HTTP).\n  nameservers:\n  - ns-153.awsdns-19.com.\n  - ns-568.awsdns-07.net.\n  - ns-1396.awsdns-46.org.\n  - ns-1562.awsdns-03.co.uk.\n  dns:\n    a: []\n    aaaa: []\n    ns_present: true\n    dnssec: false\n    ds_records: []\n    caa: []\n\
  \    mx:\n    - 1 aspmx.l.google.com.\n    - 5 alt1.aspmx.l.google.com.\n    - 5 alt2.aspmx.l.google.com.\n    - 10 alt3.aspmx.l.google.com.\n    - 10 alt4.aspmx.l.google.com.\n    spf: v=spf1 include:_spf.google.com ~all\n    dmarc: null\n  tls:\n    probed: false\n    reason: host does not resolve\n  hsts:\n    probed: false\n    reason: host does not resolve\nfindings:\n- id: no-web-surface\n  severity: informational\n  detail: Domain has no A/AAAA record; the former developer portal and documentation are offline.\n- id: dnssec-absent\n  severity: low\n  detail: No DS records published for bluevisionlabs.com.\n- id: caa-absent\n  severity: low\n  detail: No CAA records restrict certificate issuance for bluevisionlabs.com.\n- id: dmarc-absent\n  severity: medium\n  detail: No _dmarc.bluevisionlabs.com TXT record, while MX still routes mail to Google Workspace.\n- id: spf-present\n  severity: informational\n  detail: SPF published as a soft-fail (~all) allowing Google Workspace senders.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blue-vision-labs/refs/heads/main/security/blue-vision-labs-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Frontier Tech
- Augmented Reality
- Computer Vision
- Mapping
- Localization
- Spatial Computing
- Acquired
- Retired
---
