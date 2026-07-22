---
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: outpost.bio
  spf: true
hosts:
- cert_expires: Oct 17 14:51:12 2026 GMT
  host: outpost.bio
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Outpost Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Outpost Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Outpost Bio
provider_slug: outpost-bio
slug: outpost-bio-domain-security
source_filename: outpost-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: outpost.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 14:51:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: outpost.bio\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/outpost-bio/refs/heads/main/security/outpost-bio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Foundation Models
- Microbiome
- Biotechnology
- Life Sciences
- Drug Discovery
- Open Source
---
