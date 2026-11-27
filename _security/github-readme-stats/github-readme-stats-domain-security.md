---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vercel.app
  spf: true
hosts:
- cert_expires: Jan 29 11:46:09 2027 GMT
  host: github-readme-stats.vercel.app
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GitHub ReadMe Stats Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GitHub ReadMe Stats, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GitHub ReadMe Stats
provider_slug: github-readme-stats
slug: github-readme-stats-domain-security
source_filename: github-readme-stats-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: github-readme-stats.vercel.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 11:46:09 2027 GMT\n  hsts: null\ndomains:\n- domain: vercel.app\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/github-readme-stats/security/github-readme-stats-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Badges
- Developer Tools
- GitHub
- Open Source
- Open Source Projects
- Profile README
- Public APIs
- SVG
---
