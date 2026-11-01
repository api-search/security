---
description: ''
domains:
- caa:
  - 0 issue "starfieldtech.com"
  - 0 iodef "mailto:caa@eurosms.com"
  - 0 issuewild "starfieldtech.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: eurosms.com
  spf: true
hosts:
- host: eurosms.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Eurosms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EuroSms, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: EuroSms
provider_slug: eurosms
slug: eurosms-domain-security
source_filename: eurosms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eurosms.com\n  https: false\ndomains:\n- domain: eurosms.com\n  dnssec: false\n  caa:\n  - 0 issue \"starfieldtech.com\"\n  - 0 iodef \"mailto:caa@eurosms.com\"\n  - 0 issuewild \"starfieldtech.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/eurosms/security/eurosms-domain-security.yml
summary_line: DMARC
tags:
- Company
- SMS
- BulkMessaging
- API
- Slovakia
---
