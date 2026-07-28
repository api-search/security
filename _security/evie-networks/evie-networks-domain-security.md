---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: evie.com.au
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dmarc_record: v=DMARC1; p=none; pct=100; rua=mailto:dmarc@goevie.com.au
  dnssec: false
  domain: goevie.com.au
  note: 'TXT records also disclose the app-side stack: firebase=prod-evie (Firebase

    project), an Atlassian domain verification, a Google site verification and

    Microsoft 365 mail. No CAA and no DNSSEC on this domain, and DMARC is

    monitor-only (p=none) versus quarantine on evie.com.au.

    '
  spf: true
  spf_record: v=spf1 include:spf.protection.outlook.com include:_spf.firebasemail.com include:spf.mandrillapp.com -all
hosts:
- cert_expires: Sep 26 05:34:11 2026 GMT
  host: evie.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 01:15:06 2026 GMT
  cert_issuer: Google Trust Services WR3
  host: api.goevie.com.au
  hsts: false
  http_version: HTTP/2
  https: true
  note: 'Undocumented production API gateway behind the Evie Charging mobile app.

    Server headers identify Google Frontend with an Envoy/ESPv2 decorator

    (x-envoy-decorator-operation: ingress UnknownOperationName), i.e. Google

    Cloud Endpoints. Not listed in apis.yml because no public documentation,

    contract, terms or onboarding exist for it.

    '
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Evie Networks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Evie Networks, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Evie Networks
provider_slug: evie-networks
slug: evie-networks-domain-security
source_filename: evie-networks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts, extended by hand with the undocumented API host (api.goevie.com.au) found during review\nhosts:\n- host: evie.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 05:34:11 2026 GMT\n  hsts: false\n- host: api.goevie.com.au\n  https: true\n  http_version: HTTP/2\n  tls_version: TLSv1.3\n  cert_issuer: Google Trust Services WR3\n  cert_expires: Sep 13 01:15:06 2026 GMT\n  hsts: false\n  note: |\n    Undocumented production API gateway behind the Evie Charging mobile app.\n    Server headers identify Google Frontend with an Envoy/ESPv2 decorator\n    (x-envoy-decorator-operation: ingress UnknownOperationName), i.e. Google\n    Cloud Endpoints. Not listed in apis.yml because no public documentation,\n    contract, terms or onboarding exist for it.\ndomains:\n- domain: evie.com.au\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n\
  - domain: goevie.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:spf.protection.outlook.com include:_spf.firebasemail.com include:spf.mandrillapp.com -all\n  dmarc: true\n  dmarc_policy: none\n  dmarc_record: v=DMARC1; p=none; pct=100; rua=mailto:dmarc@goevie.com.au\n  note: |\n    TXT records also disclose the app-side stack: firebase=prod-evie (Firebase\n    project), an Atlassian domain verification, a Google site verification and\n    Microsoft 365 mail. No CAA and no DNSSEC on this domain, and DMARC is\n    monitor-only (p=none) versus quarantine on evie.com.au.\nfindings: |\n  Both hosts serve TLS 1.3 with valid certificates. Neither host sets HSTS.\n  The corporate domain (evie.com.au) is DNSSEC-signed with a DMARC quarantine\n  policy; the API/app domain (goevie.com.au) is neither DNSSEC-signed nor\n  CAA-protected and runs DMARC in monitor-only mode. Absence of a record is\n  recorded data, not a failed probe.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evie-networks/refs/heads/main/security/evie-networks-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Energy
- Australia
- EV Charging
- Electricity
- Utilities
- E-Mobility
- Charging Infrastructure
- Fleet
- Transport Electrification
---
