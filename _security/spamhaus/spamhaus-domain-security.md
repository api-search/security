---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: spamhaus.org
  spf: true
hosts:
- cert_expires: Dec 17 09:06:45 2026 GMT
  host: spamhaus.org
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Spamhaus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spamhaus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Spamhaus
provider_slug: spamhaus
slug: spamhaus-domain-security
source_filename: spamhaus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spamhaus.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 09:06:45 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: spamhaus.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/spamhaus/security/spamhaus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Anti-Spam
- Reputation
- DNSBL
---
