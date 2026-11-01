---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: stopforumspam.com
  spf: true
hosts:
- cert_expires: Jan  6 10:31:47 2027 GMT
  host: stopforumspam.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Stopforumspam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StopForumSpam, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: StopForumSpam
provider_slug: stopforumspam
slug: stopforumspam-domain-security
source_filename: stopforumspam-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stopforumspam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 10:31:47 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: stopforumspam.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/stopforumspam/security/stopforumspam-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Spam
- Security
- API
- Community
---
