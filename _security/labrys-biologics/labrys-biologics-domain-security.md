---
description: ''
domains:
- caa: []
  created: '2012-12-09'
  dmarc: true
  dmarc_policy: reject
  dmarc_rua: dmarc.RUA@tevapharm.com
  dnssec: false
  domain: labrysbiologics.com
  expires: '2026-12-09'
  nameservers:
  - ns3.tevapharm.com
  - ns4.tevapharm.com
  - ns5.tevapharm.com
  registrant_organization: Labrys Biologics
  registrar: Nom-iq Ltd. dba COM LAUDE
  spf: true
  spf_record: v=spf1 -all
hosts:
- a_record: 192.115.248.118
  host: labrysbiologics.com
  hsts: null
  http_port_80: closed
  https: false
  https_port_443: closed
  resolves: true
- a_record: 192.115.248.118
  host: labrysbio.com
  hsts: null
  http_port_80: closed
  https: false
  https_port_443: closed
  resolves: true
kind: domain-security
layout: security
method: probed
name: Labrys Biologics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Labrys Biologics, probed live across 2 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Labrys Biologics
provider_slug: labrys-biologics
slug: labrys-biologics-domain-security
source_filename: labrys-biologics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the registrant domain labrysbiologics.com\nnote: >-\n  labrysbiologics.com resolves but serves nothing — TCP 80 and 443 are both closed, so no\n  TLS/HSTS posture can be observed. The domain is a defended brand registration held under\n  Teva nameservers (ns3/ns4/ns5.tevapharm.com) following Teva's 2014 acquisition of Labrys\n  Biologics. The mail posture is a deliberate no-mail lockdown: SPF \"v=spf1 -all\" and DMARC\n  p=reject with aggregate reports routed to dmarc.RUA@tevapharm.com.\nhosts:\n- host: labrysbiologics.com\n  https: false\n  http_port_80: closed\n  https_port_443: closed\n  resolves: true\n  a_record: 192.115.248.118\n  hsts: null\n- host: labrysbio.com\n  https: false\n  http_port_80: closed\n  https_port_443: closed\n  resolves: true\n  a_record: 192.115.248.118\n  hsts: null\ndomains:\n- domain: labrysbiologics.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 -all\n\
  \  dmarc: true\n  dmarc_policy: reject\n  dmarc_rua: dmarc.RUA@tevapharm.com\n  nameservers:\n  - ns3.tevapharm.com\n  - ns4.tevapharm.com\n  - ns5.tevapharm.com\n  registrar: Nom-iq Ltd. dba COM LAUDE\n  registrant_organization: Labrys Biologics\n  created: '2012-12-09'\n  expires: '2026-12-09'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/labrys-biologics/refs/heads/main/security/labrys-biologics-domain-security.yml
summary_line: DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Life Sciences
- Therapeutics
- Neurology
- Clinical Research
- Acquired
---
