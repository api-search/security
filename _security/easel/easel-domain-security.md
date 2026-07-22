---
description: ''
domains:
- caa: []
  caa_note: No CAA record is published. The probe script initially recorded four values here, but `dig CAA easelapps.ai` follows the apex CNAME to Azure Static Web Apps and returns that CNAME chain (icy-sand-0a3bac010.1.azurestaticapps.net -> azurestaticapps1.trafficmanager.net -> msha-slice-1-eus2-0.msha-slice-1-eus2-0-ase.p.azurewebsites.net -> waws-prod-bn1-d5bb8b62.sip.p.azurewebsites.windows.net), not CAA data. Corrected by hand on 2026-07-20.
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: easelapps.ai
  hosting: Azure Static Web Apps (apex CNAME)
  spf: false
hosts:
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: easelapps.ai
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Easel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Easel AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: Easel AI
provider_slug: easel
slug: easel-domain-security
source_filename: easel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: easelapps.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: easelapps.ai\n  dnssec: true\n  caa: []\n  caa_note: >-\n    No CAA record is published. The probe script initially recorded four values\n    here, but `dig CAA easelapps.ai` follows the apex CNAME to Azure Static Web\n    Apps and returns that CNAME chain (icy-sand-0a3bac010.1.azurestaticapps.net\n    -> azurestaticapps1.trafficmanager.net ->\n    msha-slice-1-eus2-0.msha-slice-1-eus2-0-ase.p.azurewebsites.net ->\n    waws-prod-bn1-d5bb8b62.sip.p.azurewebsites.windows.net), not CAA data.\n    Corrected by hand on 2026-07-20.\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n  hosting: Azure Static Web Apps (apex CNAME)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/easel/refs/heads/main/security/easel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Generative AI
- Image Generation
- Avatars
- Fashion
- Virtual Try-On
- Advertising
- Computer Vision
- Consumer Applications
---
