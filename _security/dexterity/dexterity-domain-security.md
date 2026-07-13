---
api_specs:
- filename: dexterity-foresight-packing-challenge-openapi.yml
  format: yaml
  label: Dexterity Foresight Packing Challenge API
  slug: dexterity-foresight-packing-challenge
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dexterity/refs/heads/main/openapi/dexterity-foresight-packing-challenge-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "comodoca.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dexterity.ai
  spf: true
hosts:
- cert_expires: Sep 17 21:10:47 2026 GMT
  host: www.dexterity.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 15 05:05:13 2026 GMT
  host: dexterity.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dexterity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dexterity, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Dexterity
provider_slug: dexterity
slug: dexterity-domain-security
source_filename: dexterity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dexterity.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 21:10:47 2026 GMT\n  hsts: false\n- host: dexterity.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 05:05:13 2026 GMT\n  hsts: false\ndomains:\n- domain: dexterity.ai\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dexterity/refs/heads/main/security/dexterity-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Physical AI
- Industrial Robotics
- Robotics
- Warehouse Automation
- Logistics
- Manufacturing
- World Model
- Foresight
- Mech
- Dual-Arm
- Truck Loading
- Palletizing
- Depalletizing
- Singulation
- Research API
- Packing Challenge
---
