---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: urbanengines.com
  spf: true
hosts:
- host: www.urbanengines.com
  https: false
kind: domain-security
layout: security
method: probed
name: Urban Engines Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Urban Engines, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Urban Engines
provider_slug: urban-engines
slug: urban-engines-domain-security
source_filename: urban-engines-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.urbanengines.com\n  https: false\ndomains:\n- domain: urbanengines.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urban-engines/refs/heads/main/security/urban-engines-domain-security.yml
summary_line: DMARC
tags:
- Company
- Transportation
- Urban Mobility
- Data Analytics
- Mapping
- Logistics
- Defunct
---
