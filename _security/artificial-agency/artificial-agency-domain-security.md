---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: artificial.agency
  spf: true
hosts:
- cert_expires: Dec  4 15:47:48 2026 GMT
  host: www.artificial.agency
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Artificial Agency Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Artificial Agency, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Artificial Agency
provider_slug: artificial-agency
slug: artificial-agency-domain-security
source_filename: artificial-agency-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.artificial.agency\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 15:47:48 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: artificial.agency\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/artificial-agency/security/artificial-agency-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Behavior Engine
- Game Development
- AI NPCs
- Generative AI
- Unity Support
- Studio Tools
---
