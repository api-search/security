---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aeratechnology.com
  spf: true
hosts:
- cert_expires: Sep 17 02:01:46 2026 GMT
  host: www.aeratechnology.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aera Technology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aera Technology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Aera Technology
provider_slug: aera-technology
slug: aera-technology-domain-security
source_filename: aera-technology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aeratechnology.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 02:01:46 2026 GMT\n  hsts: false\ndomains:\n- domain: aeratechnology.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aera-technology/refs/heads/main/security/aera-technology-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Decision Intelligence
- Artificial Intelligence
- Enterprise Software
- Supply Chain
- Automation
- Analytics
- Agents
---
