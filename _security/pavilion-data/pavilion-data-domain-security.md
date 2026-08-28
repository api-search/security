---
description: ''
domains: []
hosts:
- caa:
    present: false
    records: []
  dmarc:
    policy: quarantine
    present: true
    record: v=DMARC1; p=quarantine; rua=mailto:spoof-quarantine@pavilion.io; ruf=mailto:spoof-quarantine@pavilion.io; pct=100; ri=86400; fo=1;
  dns:
    a:
    - 44.224.211.240
    - 44.224.118.103
    mx:
    - aspmx.l.google.com
    - alt1.aspmx.l.google.com
    - alt2.aspmx.l.google.com
    - alt3.aspmx.l.google.com
    - alt4.aspmx.l.google.com
    ns:
    - ns11.domaincontrol.com
    - ns12.domaincontrol.com
  dnssec:
    dnskey_records: 0
    ds_records: 0
    enabled: false
  host: pavilion.io
  hsts:
    note: not observable — no HTTPS response to read a Strict-Transport-Security header from
    present: null
  https:
    cert_expires: null
    observed: curl exit 28 / connection timed out; nc reports 80 and 443 closed on both A records
    reachable: false
    tcp_443: refused
    tcp_80: refused
    tls_version: null
  other_txt:
  - google-site-verification=-T8MX4jHcfmPdsfymazgoRCQhB0GZ_Am2ci2a7F_88I
  - google-site-verification=l6913O0oxPbk793YcDQ2wHzWfb0qUhqKc2q49Bop-ek
  - ZOOM_verify_d7ctiSHOSp2Hp0ly6-FXsg
  registrable_domain: pavilion.io
  spf:
    policy: ~all (softfail)
    present: true
    record: v=spf1 include:_spf.google.com include:mktomail.com include:aspmx.pardot.com include:_spf.salesforce.com ~all
kind: domain-security
layout: security
method: probed
name: Pavilion Data Domain Security
name_suffix: Domain Security
overview: Domain security posture for Pavilion, probed live across 1 host(s) and 0 registrable domain(s). 1 host(s) serve HTTPS; 1 advertise HSTS.
provider_name: Pavilion
provider_slug: pavilion-data
slug: pavilion-data-domain-security
source_filename: pavilion-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: dig + TCP/TLS probes against pavilion.io (2026-08-26)\nnote: >-\n  Pavilion Data Systems ceased operations on 2022-10-12. The registrable domain\n  pavilion.io is still registered (GoDaddy, registry expiry 2027-01-29) and its DNS\n  zone still answers, but no web server is listening: both A records (44.224.211.240,\n  44.224.118.103, AWS us-west-2) refuse connections on TCP 80 and 443. Mail records\n  are still published, so the DNS-layer findings below are real and current while the\n  HTTPS-layer findings are \"host unreachable\", not \"misconfigured\".\nhosts:\n  - host: pavilion.io\n    registrable_domain: pavilion.io\n    dns:\n      a:\n        - 44.224.211.240\n        - 44.224.118.103\n      ns:\n        - ns11.domaincontrol.com\n        - ns12.domaincontrol.com\n      mx:\n        - aspmx.l.google.com\n        - alt1.aspmx.l.google.com\n        - alt2.aspmx.l.google.com\n        - alt3.aspmx.l.google.com\n        - alt4.aspmx.l.google.com\n\
  \    https:\n      reachable: false\n      tcp_443: refused\n      tcp_80: refused\n      tls_version: null\n      cert_expires: null\n      observed: 'curl exit 28 / connection timed out; nc reports 80 and 443 closed on both A records'\n    hsts:\n      present: null\n      note: not observable — no HTTPS response to read a Strict-Transport-Security header from\n    dnssec:\n      enabled: false\n      dnskey_records: 0\n      ds_records: 0\n    caa:\n      present: false\n      records: []\n    spf:\n      present: true\n      record: 'v=spf1 include:_spf.google.com include:mktomail.com include:aspmx.pardot.com include:_spf.salesforce.com ~all'\n      policy: '~all (softfail)'\n    dmarc:\n      present: true\n      record: 'v=DMARC1; p=quarantine; rua=mailto:spoof-quarantine@pavilion.io; ruf=mailto:spoof-quarantine@pavilion.io; pct=100; ri=86400; fo=1;'\n      policy: quarantine\n    other_txt:\n      - 'google-site-verification=-T8MX4jHcfmPdsfymazgoRCQhB0GZ_Am2ci2a7F_88I'\n      -\
  \ 'google-site-verification=l6913O0oxPbk793YcDQ2wHzWfb0qUhqKc2q49Bop-ek'\n      - 'ZOOM_verify_d7ctiSHOSp2Hp0ly6-FXsg'\nregistrar:\n  name: GoDaddy.com, LLC\n  creation_date: '2016-01-29'\n  registry_expiry_date: '2027-01-29'\n  last_updated: '2026-08-12'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pavilion-data/refs/heads/main/security/pavilion-data-domain-security.yml
summary_line: HSTS
tags:
- Company
- Storage
- Flash Storage
- NVMe
- NVMe over Fabrics
- Data Infrastructure
- Enterprise Hardware
- High Performance Computing
- Defunct
---
