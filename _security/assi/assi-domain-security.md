---
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: assi.st
  ds_record: false
  mx:
  - 1 aspmx.l.google.com
  nameservers:
  - ns1.101domain.com
  - ns2.101domain.com
  - ns5.101domain.com
  spf: false
hosts:
- a_record: false
  aaaa_record: false
  cert_expires: null
  evidence: dig +short assi.st A returned no answer
  host: assi.st
  hsts: null
  https: null
  reachable: false
  tls_version: null
kind: domain-security
layout: security
method: probed
name: Assi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Assist, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Assist
provider_slug: assi
slug: assi-domain-security
source_filename: assi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS probes of assi.st (the only host in apis.yml)\nnotes: >-\n  assi.st resolves NS records but publishes no A/AAAA record, so there is no\n  reachable web host and no TLS endpoint to probe. Mail is still routed to\n  Google Workspace via MX. The company (Assist) was acquired by Conversocial in\n  March 2019 and the domain is now parked at 101domain nameservers.\nhosts:\n- host: assi.st\n  reachable: false\n  a_record: false\n  aaaa_record: false\n  https: null\n  tls_version: null\n  cert_expires: null\n  hsts: null\n  evidence: dig +short assi.st A returned no answer\ndomains:\n- domain: assi.st\n  nameservers:\n  - ns1.101domain.com\n  - ns2.101domain.com\n  - ns5.101domain.com\n  dnssec: false\n  ds_record: false\n  caa: []\n  mx:\n  - 1 aspmx.l.google.com\n  spf: false\n  dmarc: false\n  dmarc_policy: null\nfindings:\n- id: no-web-host\n  severity: informational\n  detail: No A/AAAA record; the public website is\
  \ offline.\n- id: no-dnssec\n  severity: low\n  detail: No DS record published for assi.st.\n- id: no-caa\n  severity: low\n  detail: No CAA record restricting which CAs may issue for assi.st.\n- id: no-spf\n  severity: medium\n  detail: MX still routes mail to Google Workspace but no SPF TXT record is published.\n- id: no-dmarc\n  severity: medium\n  detail: No _dmarc.assi.st TXT record, so the domain publishes no DMARC policy.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/assi/refs/heads/main/security/assi-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Conversational Commerce
- Chatbots
- Messaging
- Customer Experience
- Artificial Intelligence
- Acquired
---
