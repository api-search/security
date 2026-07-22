---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pillar.tech
  spf: true
hosts:
- cert_expires: Feb 13 02:27:51 2027 GMT
  host: pillar.tech
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Pillar Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pillar Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Pillar Technologies
provider_slug: pillar-technologies
slug: pillar-technologies-domain-security
source_filename: pillar-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pillar.tech\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 13 02:27:51 2027 GMT\n  hsts: false\ndomains:\n- domain: pillar.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pillar-technologies/refs/heads/main/security/pillar-technologies-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Construction
- IoT
- Sensors
- Environmental Monitoring
- Jobsite Safety
- Analytics
- Real Estate Technology
---
