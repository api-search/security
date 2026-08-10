---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dmarc_rua: mailto:abuse@gatik.ai
  dnssec: false
  domain: gatik.ai
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:_spf.psm.knowbe4.com include:6767982.spf08.hubspotemail.net ~all
hosts:
- cert_expires: Sep  6 00:26:57 2026 GMT
  host: gatik.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  server: Vercel
  tls_version: TLSv1.3
- cert_expires: Sep  6 00:37:34 2026 GMT
  host: archive.gatik.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  note: legacy WordPress site; carries about/safety/news/careers/legal pages the current gatik.ai navigation links out to
  server: cloudflare
  tls_version: TLSv1.3
- cert_expires: Oct  7 19:39:44 2026 GMT
  host: news.gatik.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  note: 301-redirects to https://archive.gatik.ai/
  server: cloudflare
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gatik Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gatik, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gatik
provider_slug: gatik
slug: gatik-domain-security
source_filename: gatik-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts (0-working/probe-domain-security.py,\n  extended by hand for the archive/news hosts and for the HSTS header, which the\n  script's HEAD request could not read)\nhosts:\n- host: gatik.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 00:26:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  server: Vercel\n- host: archive.gatik.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 00:37:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  server: cloudflare\n  note: legacy WordPress site; carries about/safety/news/careers/legal pages the\n    current gatik.ai navigation links out to\n- host: news.gatik.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 19:39:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  server: cloudflare\n  note: 301-redirects to https://archive.gatik.ai/\ndomains:\n- domain: gatik.ai\n  dnssec: false\n  caa: []\n\
  \  spf: true\n  spf_record: v=spf1 include:_spf.google.com include:_spf.psm.knowbe4.com include:6767982.spf08.hubspotemail.net\n    ~all\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_rua: mailto:abuse@gatik.ai\nobservations:\n- HSTS is enforced on every reachable host with a two-year max-age.\n- No DNSSEC and no CAA records are published for gatik.ai.\n- DMARC is published at p=quarantine (not reject) with an aggregate-report address.\n- gatik.ai carries a Cloudflare wildcard DNS record, so arbitrary subdomains\n  (api., docs., developer., app., and a nonsense control name) all resolve to the\n  same Cloudflare IPs and fail the TLS handshake with HTTP 525. Those 525s are a\n  wildcard artifact, not a gated API host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gatik/refs/heads/main/security/gatik-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Autonomous Vehicles
- Autonomous Trucking
- Logistics
- Freight
- Middle Mile
- Supply Chain
- Transportation
- Robotics
- Artificial Intelligence
---
