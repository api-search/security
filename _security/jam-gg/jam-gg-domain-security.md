---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jam.gg
  spf: true
hosts:
- host: jam.gg
  https: false
kind: domain-security
layout: security
method: probed
name: Jam Gg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jam.gg, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Jam.gg
provider_slug: jam-gg
slug: jam-gg-domain-security
source_filename: jam-gg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jam.gg\n  https: false\ndomains:\n- domain: jam.gg\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\nx-findings:\n  note: >-\n    Added by hand on 2026-08-17 alongside the mechanical probe. The probe's boolean fields are\n    correct as booleans (a record of each type is present) but both records are malformed in ways\n    that make them non-functional, which the booleans cannot express. Recorded here rather than by\n    overwriting the probe's output.\n  https_false_detail: >-\n    `https: false` here is not a missing-redirect finding — the TLS handshake itself never completes.\n    jam.gg (Netlify / AWS Global Accelerator, 75.2.70.75 and 99.83.190.102) answers the ClientHello\n    with TLS alert 80 (internal_error), the signature of a hostname with no provisioned certificate.\n    www.jam.gg (proxy-ssl.webflow.com) answers with\
  \ TLS alert 40 (handshake_failure). Port 80 on both\n    still returns 301 into that dead HTTPS origin, so no client can reach the site at all.\n  spf: >-\n    RFC 7208 section 3.2 violation — jam.gg publishes TWO v=spf1 TXT records:\n    \"v=spf1 include:secureserver.net -all\" and\n    \"v=spf1 include:_spf.mailersend.net include:secureserver.net -all\".\n    More than one SPF record means a checking implementation MUST return permerror, so SPF\n    evaluation fails for the domain despite a record being present.\n  dmarc: >-\n    RFC 7489 violation — the _dmarc.jam.gg TXT record is\n    \"Value: v=DMARC1; p=none; rua=mailto:jules@jam.gg\". The literal \"Value: \" prefix means the record\n    does not begin with the required v=DMARC1 tag, so conforming receivers discard it as not a DMARC\n    record. The effective policy is therefore no DMARC at all, not p=none. This looks like a control\n    panel form field label pasted into the record value.\n  mail: jam.gg MX points at jam-gg.mail.protection.outlook.com\
  \ (Microsoft 365); registrar/DNS is GoDaddy (domaincontrol.com nameservers).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jam-gg/refs/heads/main/security/jam-gg-domain-security.yml
summary_line: DMARC
tags:
- Company
- Gaming
- Cloud Gaming
- Games
- Game Development
- Emulation
- SDK
- WebRTC
- France
---
