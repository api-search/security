---
description: ''
domains:
- caa:
  - 0 issue "digicert.com; account=b34fd286db03ccad020f0a75010dd75544eaf2b967195b4becb6460c924d35c9"
  - 0 iodef "mailto:pkiadmin@dell.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: scaleio.com
  spf: true
hosts:
- host: scaleio.com
  https: false
kind: domain-security
layout: security
method: probed
name: Scaleio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scaleio, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Scaleio
provider_slug: scaleio
slug: scaleio-domain-security
source_filename: scaleio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scaleio.com\n  https: false\ndomains:\n- domain: scaleio.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; account=b34fd286db03ccad020f0a75010dd75544eaf2b967195b4becb6460c924d35c9\"\n  - 0 iodef \"mailto:pkiadmin@dell.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scaleio/refs/heads/main/security/scaleio-domain-security.yml
summary_line: DMARC
tags:
- Company
- Storage
- Software-Defined Storage
- Block Storage
- Dell EMC
- Acquired
---
