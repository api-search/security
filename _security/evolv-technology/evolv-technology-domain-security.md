---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: evolvtechnology.com
  spf: true
hosts:
- cert_expires: Oct 14 16:01:51 2026 GMT
  host: www.evolvtechnology.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Evolv Technology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Evolv Technology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Evolv Technology
provider_slug: evolv-technology
slug: evolv-technology-domain-security
source_filename: evolv-technology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.evolvtechnology.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 16:01:51 2026 GMT\n  hsts: null\ndomains:\n- domain: evolvtechnology.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evolv-technology/refs/heads/main/security/evolv-technology-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Security
- Physical Security
- Weapons Detection
- Screening
- Artificial Intelligence
- Sensor Fusion
- Public Safety
---
