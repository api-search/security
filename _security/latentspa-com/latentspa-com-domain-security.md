---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: latentspa.com
  spf: true
hosts:
- cert_expires: Jan 16 23:30:24 2027 GMT
  host: latentspa.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Latent Spa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Latent Spa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Latent Spa
provider_slug: latentspa-com
slug: latentspa-com-domain-security
source_filename: latentspa-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: latentspa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 23:30:24 2027 GMT\n  hsts: false\ndomains:\n- domain: latentspa.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/latentspa-com/security/latentspa-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Retreat
- Open Access
- Experience
---
