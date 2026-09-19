---
description: ''
domains:
- caa: []
  caa_note: No CAA record is published. `dig +short CAA agilebio.com.cn` answers only with the apex CNAME (agilebio.gotoip11.com.), which probe-domain-security.py 0.x records as a CAA value; the authoritative answer section carries a CNAME RR and no CAA RR. Hand corrected 2026-09-14 — see the note in the enrichment report.
  dmarc: false
  dnssec: false
  domain: agilebio.com.cn
  spf: true
hosts:
- host: agilebio.com.cn
  https: false
  note: No TLS listener on port 443. The only site this company operates is served over plaintext HTTP; https://agilebio.com.cn/ does not connect at all (curl exit 7 / HTTP code 000). The apex is a CNAME to agilebio.gotoip11.com -> web.s1312.vhostgo.com (211.149.233.219), Chinese shared hosting.
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aijieboya Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aijieboya, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Aijieboya
provider_slug: aijieboya
slug: aijieboya-domain-security
source_filename: aijieboya-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agilebio.com.cn\n  https: false\n  note: >-\n    No TLS listener on port 443. The only site this company operates is served over\n    plaintext HTTP; https://agilebio.com.cn/ does not connect at all (curl exit 7 /\n    HTTP code 000). The apex is a CNAME to agilebio.gotoip11.com -> web.s1312.vhostgo.com\n    (211.149.233.219), Chinese shared hosting.\ndomains:\n- domain: agilebio.com.cn\n  dnssec: false\n  caa: []\n  caa_note: >-\n    No CAA record is published. `dig +short CAA agilebio.com.cn` answers only with the\n    apex CNAME (agilebio.gotoip11.com.), which probe-domain-security.py 0.x records as a\n    CAA value; the authoritative answer section carries a CNAME RR and no CAA RR. Hand\n    corrected 2026-09-14 — see the note in the enrichment report.\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aijieboya/refs/heads/main/security/aijieboya-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Chromatography
- Laboratory Instruments
- Sample Preparation
- Separation and Purification
- Scientific Instruments
- Life Sciences
- Clinical Mass Spectrometry
- Biotechnology
- Manufacturing
- China
---
