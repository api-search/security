---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dura.software
  spf: true
hosts:
- cert_expires: Dec 18 20:30:45 2026 GMT
  host: dura.software
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dura Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dura Software, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Dura Software
provider_slug: dura-software
slug: dura-software-domain-security
source_filename: dura-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dura.software\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 20:30:45 2026 GMT\n  hsts: false\ndomains:\n- domain: dura.software\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/dura-software/security/dura-software-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Acquisitions
- Software
- Managed Services
- Technology
---
