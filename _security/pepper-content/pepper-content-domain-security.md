---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pepper.inc
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: peppercontent.io
  note: Email authentication is configured on the legacy peppercontent.io domain but NOT on the current primary brand domain pepper.inc, which has neither SPF nor DMARC. The company rebranded onto a domain with weaker email posture than the one it left.
  spf: true
  spf_policy: -all
hosts:
- cert_expires: Oct 27 12:41:45 2026 GMT
  host: www.pepper.inc
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 06:43:22 2026 GMT
  host: platform.pepper.inc
  hsts: false
  https: true
  role: authenticated platform single-page application (Cloudflare Pages)
  tls_version: TLSv1.3
- cert_expires: Sep 17 13:57:29 2026 GMT
  host: hub.peppercontent.io
  hsts: false
  https: true
  role: first-party API gateway (Kong 3.6.1, Google Cloud upstream)
  tls_version: TLSv1.3
- cert_expires: Nov  9 05:07:33 2026 GMT
  host: www.peppercontent.io
  hsts: false
  https: true
  role: legacy brand domain, serves the pepper.inc marketing site
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pepper Content Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pepper Content, probed live across 4 host(s) and 2 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Pepper Content
provider_slug: pepper-content
slug: pepper-content-domain-security
source_filename: pepper-content-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: >-\n  live DNS/TLS/HTTP probes, 2026-08-13. www.pepper.inc + pepper.inc from\n  0-working/probe-domain-security.py; platform.pepper.inc, hub.peppercontent.io,\n  www.peppercontent.io and the peppercontent.io domain probed directly this pass after\n  contract discovery surfaced them.\nhosts:\n- host: www.pepper.inc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 12:41:45 2026 GMT\n  hsts: false\n- host: platform.pepper.inc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 06:43:22 2026 GMT\n  hsts: false\n  role: authenticated platform single-page application (Cloudflare Pages)\n- host: hub.peppercontent.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 13:57:29 2026 GMT\n  hsts: false\n  role: first-party API gateway (Kong 3.6.1, Google Cloud upstream)\n- host: www.peppercontent.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 05:07:33 2026 GMT\n  hsts: false\n  role:\
  \ legacy brand domain, serves the pepper.inc marketing site\ndomains:\n- domain: pepper.inc\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: peppercontent.io\n  dnssec: false\n  caa: []\n  spf: true\n  spf_policy: '-all'\n  dmarc: true\n  dmarc_policy: quarantine\n  note: >-\n    Email authentication is configured on the legacy peppercontent.io domain but NOT on\n    the current primary brand domain pepper.inc, which has neither SPF nor DMARC. The\n    company rebranded onto a domain with weaker email posture than the one it left.\nfindings:\n- No host sets HSTS.\n- No domain publishes DNSSEC or CAA records.\n- pepper.inc publishes neither SPF nor DMARC.\n- Every host negotiates TLS 1.3 with a current certificate.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pepper-content/refs/heads/main/security/pepper-content-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai Ml
- Content Marketing
- SEO
- Generative Engine Optimization
- Content Strategy
- Creative
- Marketing
---
