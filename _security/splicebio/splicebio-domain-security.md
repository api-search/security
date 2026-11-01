---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: splice.bio
  spf: true
hosts:
- cert_expires: Dec 22 01:26:32 2026 GMT
  host: splice.bio
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Splicebio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SpliceBio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SpliceBio
provider_slug: splicebio
slug: splicebio-domain-security
source_filename: splicebio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: splice.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 01:26:32 2026 GMT\n  hsts: false\ndomains:\n- domain: splice.bio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/splicebio/security/splicebio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Gene-Editing
- Synthetic-Biology
- APIs
---
