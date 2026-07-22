---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dreamgroup.com
  spf: true
hosts:
- cert_expires: Sep 14 14:39:35 2026 GMT
  host: dreamgroup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dream Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dream, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Dream
provider_slug: dream
slug: dream-domain-security
source_filename: dream-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dreamgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 14:39:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dreamgroup.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dream/refs/heads/main/security/dream-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Security
- Cybersecurity
- Artificial Intelligence
- Sovereign AI
- National Security
- Critical Infrastructure
- GovTech
---
