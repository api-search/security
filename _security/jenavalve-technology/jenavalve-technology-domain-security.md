---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jenavalve.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: discover-ar.com
  spf: true
hosts:
- cert_expires: Oct 25 17:16:08 2026 GMT
  host: jenavalve.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 17:16:02 2026 GMT
  host: discover-ar.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Jenavalve Technology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JenaValve Technology, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: JenaValve Technology
provider_slug: jenavalve-technology
slug: jenavalve-technology-domain-security
source_filename: jenavalve-technology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jenavalve.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 17:16:08 2026 GMT\n  hsts: false\n- host: discover-ar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 17:16:02 2026 GMT\n  hsts: false\ndomains:\n- domain: jenavalve.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: discover-ar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jenavalve-technology/refs/heads/main/security/jenavalve-technology-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Medical Devices
- Healthcare
- Cardiology
- Structural Heart
- TAVR
- Aortic Regurgitation
- Aortic Stenosis
- Heart Valves
- Clinical Trials
- Patient Education
- Private Company
---
