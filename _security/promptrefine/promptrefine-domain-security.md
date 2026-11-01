---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: promptrefine.com
  spf: true
hosts:
- cert_expires: Dec  2 09:17:02 2026 GMT
  host: promptrefine.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Promptrefine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prompt Refine, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Prompt Refine
provider_slug: promptrefine
slug: promptrefine-domain-security
source_filename: promptrefine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: promptrefine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 09:17:02 2026 GMT\n  hsts: null\ndomains:\n- domain: promptrefine.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/promptrefine/security/promptrefine-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Prompt Engineering
- Collaboration
- Analytics
---
