---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: empirix.com
  spf: true
hosts:
- cert_expires: Sep 21 19:31:46 2026 GMT
  host: www.empirix.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Empirix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Empirix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Empirix
provider_slug: empirix
slug: empirix-domain-security
source_filename: empirix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.empirix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 19:31:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: empirix.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/empirix/refs/heads/main/security/empirix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Infrastructure
- Network Testing
- Contact Center
- Monitoring
- Quality Assurance
- Telecommunications
- Customer Experience
---
