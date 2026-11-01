---
description: ''
domains:
- caa:
  - 0 issuewild ";"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: checkmk.com
  spf: true
hosts:
- cert_expires: Dec 28 00:26:16 2026 GMT
  host: checkmk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Checkmk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Checkmk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Checkmk
provider_slug: checkmk
slug: checkmk-domain-security
source_filename: checkmk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: checkmk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 00:26:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: checkmk.com\n  dnssec: true\n  caa:\n  - 0 issuewild \";\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/checkmk/security/checkmk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Monitoring
- Observability
- IT Infrastructure
- Open Source
- SaaS
---
