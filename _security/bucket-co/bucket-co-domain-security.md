---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bucket.co
  spf: true
hosts:
- cert_expires: Jan 18 16:26:38 2027 GMT
  host: bucket.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bucket Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bucket, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bucket
provider_slug: bucket-co
slug: bucket-co-domain-security
source_filename: bucket-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bucket.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 16:26:38 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bucket.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/bucket-co/security/bucket-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Feature Flags
- SaaS
- Developer Tools
- SDKs
- Integrations
---
