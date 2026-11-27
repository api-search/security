---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ai-rechtshulp.nl
  spf: true
hosts:
- cert_expires: Jan  9 08:12:49 2027 GMT
  host: ai-rechtshulp.nl
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AI Rechtshulp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AI Rechtshulp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AI Rechtshulp
provider_slug: ai-rechtshulp-nl
slug: ai-rechtshulp-nl-domain-security
source_filename: ai-rechtshulp-nl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ai-rechtshulp.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 08:12:49 2027 GMT\n  hsts: false\ndomains:\n- domain: ai-rechtshulp.nl\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/ai-rechtshulp-nl/security/ai-rechtshulp-nl-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Legal Tech
- Netherlands
- Law
- Search
---
