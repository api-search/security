---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: planswift.com
  spf: true
hosts:
- cert_expires: Oct 29 16:07:11 2026 GMT
  host: www.planswift.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Planswift Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PlanSwift, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PlanSwift
provider_slug: planswift
slug: planswift-domain-security
source_filename: planswift-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.planswift.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 29 16:07:11 2026 GMT\n  hsts: false\ndomains:\n- domain: planswift.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/planswift/refs/heads/main/security/planswift-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Construction
- Takeoff
- Estimating
- Desktop Software
- Plugin SDK
- OLE Automation
- COM
- Scripting
- ConstructConnect
- No Public Web API
---
