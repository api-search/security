---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: smirnovlabs.com
  spf: true
hosts:
- cert_expires: Jan  1 11:16:01 2027 GMT
  host: smirnovlabs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Smirnovlabs Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for smirnovlabs-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: smirnovlabs-com
provider_slug: smirnovlabs-com
slug: smirnovlabs-com-domain-security
source_filename: smirnovlabs-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: smirnovlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 11:16:01 2027 GMT\n  hsts: false\ndomains:\n- domain: smirnovlabs.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/smirnovlabs-com/security/smirnovlabs-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- AI
- Software Engineering
- Custom Software
- Fractional CTO
- Machine Learning
---
